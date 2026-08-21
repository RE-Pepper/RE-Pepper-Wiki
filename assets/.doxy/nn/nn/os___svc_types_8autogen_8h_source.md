

# File os\_SvcTypes.autogen.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**os**](dir_53922fdb85244c81a863dd6ad700ec31.md) **>** [**os\_SvcTypes.autogen.h**](os___svc_types_8autogen_8h.md)

[Go to the documentation of this file](os___svc_types_8autogen_8h.md)


```C++
#pragma once

#include <nn/os/os_MemoryTypes.h>

namespace nn {
namespace os {

typedef void (*ThreadFunc)(uptr); // 37

struct MemoryInfo
{
        uptr        baseAddress;
        size_t      size;
        bit32       permission;
        MemoryState state;
};

struct PageInfo
{
        bit32 flags;
};

} // namespace os
} // namespace nn
```


