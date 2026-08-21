

# File nstd\_Printf.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**nstd**](dir_670efa06400c5a7c70bc1499710bffc9.md) **>** [**nstd\_Printf.h**](nstd___printf_8h.md)

[Go to the documentation of this file](nstd___printf_8h.md)


```C++
#pragma once

#ifdef __cplusplus

namespace nn {
namespace nstd {

s32 TVSNPrintf (char* dst, size_t len, const char* fmt, va_list vlist);
s32 TSNPrintf (char* dst, size_t len, const char* fmt, ...);
s32 TSPrintf (char* dst, const char* fmt, ...);

} // namespace nstd
} // namespace nn

#else

extern "C" {

s32 nnnstdTVSNPrintf (char* dst, size_t len, const char* fmt, va_list vlist);
s32 nnnstdTSNPrintf (char* dst, size_t len, const char* fmt, ...);
s32 nnnstdTSPrintf (char* dst, const char* fmt, ...);
}

#endif
```


