

# File os\_ThreadLocalStorage.cpp

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**os**](dir_56153499d95e77076f83f9f8405b15c2.md) **>** [**os\_ThreadLocalStorage.cpp**](os___thread_local_storage_8cpp.md)

[Go to the documentation of this file](os___thread_local_storage_8cpp.md)


```C++
#include <nn/assert.h>
#include <nn/os/CTR/os_ErrorHandler.h>
#include <nn/os/CTR/os_ThreadLocalRegion.h>
#include <nn/os/os_Result.h>
#include <nn/os/os_ThreadLocalStorage.h>

RP_SHUTUP

namespace nn {
namespace os {

#define TLS_NUM 16 // from assert

namespace {
typedef CTR::ThreadLocalRegion ThreadLocalBuffer; // 32

inline ThreadLocalBuffer* GetThreadLocalBuffer() // 34
{
        return CTR::GetThreadLocalRegion();
}

var(nn::os, sTLSMap, u16) = 0;

inline bool IsMappedIndex(s32 index) // 64
{
       return (sTLSMap >> index) & 1;
}

inline s32 SearchFreeTLSIndex() // 74
{
        for (int i = 0; i < TLS_NUM; ++i) {
            if (!IsMappedIndex(i)){
                return i;
            }
        }
        return -1;
}

inline s32 AllocateTLSIndex() // 92
{
        s32 index = SearchFreeTLSIndex();
        if (index >= 0 && index < TLS_NUM) {
            sTLSMap |= (1 << index);
        }
        return index;
}

inline s32 FreeTLSIndex(int index) // 107
{
        if (!IsMappedIndex(index))
        {
            return -1;
        }
        return sTLSMap &= ~(1 << index);
}
}

ThreadLocalStorage::ThreadLocalStorage() {
    m_Index = AllocateTLSIndex(); // 120

    NN_ASSERT_SDK_MSG(m_Index >= 0, "Out of Thread Local Storage Slot."); // 122
    if(m_Index < 0) {
        NN_OS_HANDLE_ERROR(ResultExceedTlsLimit());
    }
}

ThreadLocalStorage::~ThreadLocalStorage() {
    NN_ASSERT_SDK(m_Index >= 0 && m_Index < TLS_NUM); // 127
    NN_ASSERT_SDK(IsMappedIndex(m_Index)) // 128

    FreeTLSIndex(m_Index);
}

uptr ThreadLocalStorage::GetValue() const
{
    NN_ASSERT_SDK(m_Index >= 0 && m_Index < TLS_NUM); // 202
    NN_ASSERT_SDK(IsMappedIndex(m_Index)); // 203

    if (IsMappedIndex(m_Index))
    {
        return GetThreadLocalBuffer()->tls[m_Index];
    } else {
        return 0;
    }
}

void ThreadLocalStorage::SetValue(uptr value)
{
    NN_ASSERT_SDK(m_Index >= 0 && m_Index < TLS_NUM); // 210
    NN_ASSERT_SDK(IsMappedIndex(m_Index)); // 211

    if (IsMappedIndex(m_Index)) {
        GetThreadLocalBuffer()->tls[m_Index] = value;
    }
}

void ThreadLocalStorage::ClearAllSlots() {
    ThreadLocalBuffer& tlr = *GetThreadLocalBuffer();

    for( int i = 0; i < TLS_NUM; ++i )
    {
        tlr.tls[i] = 0;
    }

}

} // namespace os
} // namespace nn
```


