

# File dbg\_Break.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**dbg**](dir_8674e25a187048eae8b9b07d931da2b2.md) **>** [**dbg\_Break.h**](dbg___break_8h.md)

[Go to the documentation of this file](dbg___break_8h.md)


```C++
#pragma once

#include <nn/Result.h>
#include <nn/dbg/dbg_Enum.h>

#ifdef __cplusplus
extern "C" {
#endif

nnResult nndbgBreak(nndbgBreakReason reason);
void     nndbgPanic();
void     nndbgBreakWithMessage_(nndbgBreakReason reason, const char* filename, int lineno, const char* fmt, ...);
void     nndbgBreakWithTMessage_(nndbgBreakReason reason, const char* filename, int lineno, const char* fmt, ...);
void     nndbgBreakWithResultMessage_(nndbgBreakReason reason, nnResult result, const char* filename, int lineno, const char* fmt, ...);
void     nndbgBreakWithResultTMessage_(nndbgBreakReason reason, nnResult result, const char* filename, int lineno, const char* fmt, ...);

#ifdef __cplusplus
}
#endif

namespace nn {
namespace dbg {

typedef void (*BreakHandler)(BreakReason reason, const Result* pResult, const char* filename, int lineno, const char* message, va_list vlist);

Result Break(BreakReason reason);
void   Panic();

inline Result Break()
{
        return Break(BREAK_REASON_PANIC);
}

} // namespace dbg
} // namespace nn

```


