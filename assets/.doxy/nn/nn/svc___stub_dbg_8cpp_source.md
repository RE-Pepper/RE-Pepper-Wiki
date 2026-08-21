

# File svc\_StubDbg.cpp

[**File List**](files.md) **>** [**ARM**](dir_e721d6d0970cd65c940d1e7140f4d855.md) **>** [**svc\_StubDbg.cpp**](svc___stub_dbg_8cpp.md)

[Go to the documentation of this file](svc___stub_dbg_8cpp.md)


```C++
#include <nn/svc/svc_StubDbg.h>

namespace nn {
namespace svc {

Result
asm_ext(Break, ".nn.svc.Break")(nn::dbg::BreakReason reason) {
  svc 0x3c;
  bx lr;
}

Result asm_ext(OutputDebugString, ".nn.svc.OutputDebugString")(void const *data, int length) {
  svc 0x3d;
  bx lr;
}

} // namespace svc
} // namespace nn
```


