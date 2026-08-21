

# File svc\_Inlines.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**svc**](dir_c1b0279480f3283373e7c3eb28175a75.md) **>** [**svc\_Inlines.h**](svc___inlines_8h.md)

[Go to the documentation of this file](svc___inlines_8h.md)


```C++
#pragma once

#include <nn/Handle.h>
#include <nn/Result.h>
#include <nn/svc/svc_Stub.h>

namespace nn {
namespace svc {

inline Result WaitSynchronization(s32* pOut, Handle* handles, s32 numHandles, bool waitAll, s64 timeout)
{
        return WaitSynchronizationN(pOut, handles, numHandles, waitAll, timeout);
}

} // namespace svc
} // namespace nn

```


