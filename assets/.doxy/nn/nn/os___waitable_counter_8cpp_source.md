

# File os\_WaitableCounter.cpp

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**os**](dir_56153499d95e77076f83f9f8405b15c2.md) **>** [**os\_WaitableCounter.cpp**](os___waitable_counter_8cpp.md)

[Go to the documentation of this file](os___waitable_counter_8cpp.md)


```C++
#include <nn/assert.h>
#include <nn/os/os_WaitableCounter.h>
#include <nn/svc/svc_Stub.h>

namespace nn {
namespace os {

nnHandle WaitableCounter::s_Handle = { 0 };

void WaitableCounter::Initialize ()
{
        if (s_Handle.value == INVALID_HANDLE_VALUE.value) {
                Handle h;
                Result ret = svc::CreateAddressArbiter (&h);
                NN_ASSERT_SDK (ret.IsSuccess ());
                if (ret.IsSuccess ()) {
                        s_Handle = h;
                }
        }
}
void WaitableCounter::Finalize ()
{
        // UNUSED
}

} // namespace os
} // namespace nn
```


