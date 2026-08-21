

# File dbg\_Break.cpp

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**dbg**](dir_f5f58bbdde99f1620da85a5357502216.md) **>** [**dbg\_Break.cpp**](dbg___break_8cpp.md)

[Go to the documentation of this file](dbg___break_8cpp.md)


```C++
#include <cstdarg>
#include <nn/dbg/dbg_Break.h>
#include <nn/dbg/dbg_DebugString.h>
#include <nn/dbg/dbg_PrintResult.h>
#include <nn/svc/svc_StubDbg.h>

#include "nn/dbg/dbg_Enum.h"

RP_SHUTUP

namespace nn {
namespace dbg {

namespace {
var(nn::dbg, s_pBreakHandler, BreakHandler) = NULL;
} // namespace

void PrintErrorMessageHeader(nndbgBreakReason reason, const char* filename, int lineno)
{
        detail::TPrintf("----\n");
        if (reason == NN_DBG_BREAK_REASON_ASSERT) {
            detail::TPrintf("Assertion failure at %s:%d\n  ", filename, lineno);
        } else {
            detail::TPrintf("Panic at %s:%d\n  ", filename, lineno);
        }
}

Result Break(BreakReason reason)
{
        return nn::svc::Break(reason);
}

void Panic()
{
        // TODO
}

} // namespace dbg
} // namespace nn

extern "C" {

nnResult nndbgBreak(nndbgBreakReason reason)
{
        return nn::dbg::Break((nn::dbg::BreakReason)reason);
}

void nndbgPanic()
{
        nn::dbg::Panic();
}

void nndbgBreakWithMessage_(nndbgBreakReason reason, const char* filename, int lineno, const char* fmt, ...)
{
        va_list arg;
        va_start(arg, fmt);
        nn::dbg::PrintErrorMessageHeader(reason, filename, lineno);
        nn::dbg::detail::VPrintf(fmt, arg);
        nn::dbg::detail::TPrintf("\n");
        va_end(arg);
        nndbgBreak(reason);
}

void nndbgBreakWithTMessage_(nndbgBreakReason reason, const char* filename, int lineno, const char* fmt, ...)
{
        va_list arg;
        va_start(arg, fmt);
        nn::dbg::PrintErrorMessageHeader(reason, filename, lineno);
        nn::dbg::detail::TVPrintf(fmt, arg);
        nn::dbg::detail::TPrintf("\n");
        va_end(arg);
        nndbgBreak(reason);
}

void nndbgBreakWithResultMessage_(nndbgBreakReason reason, nnResult result, const char* filename, int lineno, const char* fmt, ...)
{
        va_list arg;
        va_start(arg, fmt);
        nn::dbg::PrintErrorMessageHeader(reason, filename, lineno);
        nn::dbg::detail::VPrintf(fmt, arg);
        nn::dbg::detail::TPrintf("\n");
        nn::dbg::detail::PrintResult(result);
        va_end(arg);
        nndbgBreak(reason);
}

void nndbgBreakWithResultTMessage_(nndbgBreakReason reason, nnResult result, const char* filename, int lineno, const char* fmt, ...)
{
        va_list arg;
        va_start(arg, fmt);
        nn::dbg::PrintErrorMessageHeader(reason, filename, lineno);
        nn::dbg::detail::TVPrintf(fmt, arg);
        nn::dbg::detail::TPrintf("\n");
        nn::dbg::detail::TPrintResult(result);
        va_end(arg);
        nndbgBreak(reason);
}
}

```


