

# File os\_MemoryTypes.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**os**](dir_53922fdb85244c81a863dd6ad700ec31.md) **>** [**os\_MemoryTypes.h**](os___memory_types_8h.md)

[Go to the documentation of this file](os___memory_types_8h.md)


```C++
#pragma once

namespace nn {
namespace os {

enum MemoryState
{
        MEMORY_STATE_FREE       = 0,
        MEMORY_STATE_RESERVED   = 1,
        MEMORY_STATE_IO         = 2,
        MEMORY_STATE_STATIC     = 3,
        MEMORY_STATE_CODE       = 4,
        MEMORY_STATE_PRIVATE    = 5,
        MEMORY_STATE_SHARED     = 6,
        MEMORY_STATE_CONTINUOUS = 7,
        MEMORY_STATE_ALIASED    = 8,
        MEMORY_STATE_ALIAS      = 9,
        MEMORY_STATE_ALIAS_CODE = 10,
        MEMORY_STATE_LOCKED     = 11,
        MEMORY_STATE_MAX_BITS   = 2147483648,
};

} // namespace os
} // namespace nn
```


