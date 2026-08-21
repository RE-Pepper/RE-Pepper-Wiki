

# File os\_Semaphore.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**os**](dir_53922fdb85244c81a863dd6ad700ec31.md) **>** [**os\_Semaphore.h**](os___semaphore_8h.md)

[Go to the documentation of this file](os___semaphore_8h.md)


```C++
#pragma once

#include <nn/os/os_Synchronization.h>

namespace nn {
namespace os {

struct Semaphore : InterruptEvent
{
        Semaphore () {}
        ~Semaphore () {}

        void Acquire () { WaitOne (); }
};
static_assert_ (sizeof (Semaphore) == 0x4);

} // namespace os
} // namespace nn
```


