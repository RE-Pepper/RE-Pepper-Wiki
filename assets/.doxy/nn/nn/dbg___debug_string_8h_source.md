

# File dbg\_DebugString.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**dbg**](dir_8674e25a187048eae8b9b07d931da2b2.md) **>** [**dbg\_DebugString.h**](dbg___debug_string_8h.md)

[Go to the documentation of this file](dbg___debug_string_8h.md)


```C++
#pragma once

#ifdef __cplusplus

namespace nn {
namespace dbg {
namespace detail {

void PutString (const char* text, int length);
void PutString (const char* text);
void VPrintf (const char* fmt, va_list arg);
void TVPrintf (const char* fmt, va_list arg);
void Printf (const char* fmt, ...);
void TPrintf (const char* fmt, ...);

} // namespace detail
} // namespace dbg
} // namespace nn

#else

extern "C" {

void nndbgPrintWarning_ (const char* filename, int lineno, const char* fmt, ...);
void nndbgTPrintWarning_ (const char* filename, int lineno, const char* fmt, ...);
void nndbgDetailPutString (const char* text, int length);
void nndbgDetailVPrintf (const char* fmt, va_list arg);
void nndbgDetailTVPrintf (const char* fmt, va_list arg);
void nndbgDetailPrintf (const char* fmt, ...);
void nndbgDetailTPrintf (const char* fmt, ...);
}

#endif
```


