

# File os\_ThreadLocalStorage.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**os**](dir_53922fdb85244c81a863dd6ad700ec31.md) **>** [**os\_ThreadLocalStorage.h**](os___thread_local_storage_8h.md)

[Go to the documentation of this file](os___thread_local_storage_8h.md)


```C++
#pragma once

namespace nn {
namespace os {

class ThreadLocalStorage
{
private:
        s32 m_Index;

public:
        ThreadLocalStorage();
        ~ThreadLocalStorage();

        uptr GetValue() const;
        void SetValue(uptr);

        static void ClearAllSlots();
};

static_assert_(sizeof(ThreadLocalStorage) == 0x4);

} // namespace os
} // namespace nn
```


