

# File svc\_StubDbg.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**svc**](dir_c1b0279480f3283373e7c3eb28175a75.md) **>** [**svc\_StubDbg.h**](svc___stub_dbg_8h.md)

[Go to the documentation of this file](svc___stub_dbg_8h.md)


```C++
#pragma once

#include <nn/Result.h>
#include <nn/dbg/dbg_Enum.h>

namespace nn {
namespace svc {

Result Break (nn::dbg::BreakReason reason);
Result OutputDebugString (void const* data, int length);

} // namespace svc
} // namespace nn
```


