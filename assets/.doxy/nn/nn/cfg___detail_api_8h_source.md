

# File cfg\_DetailApi.h

[**File List**](files.md) **>** [**cfg**](dir_d61dd7901f361aace8efbc35eb1e8191.md) **>** [**CTR**](dir_6286be2e3839b9d14dbaf851f98cbdb4.md) **>** [**cfg\_DetailApi.h**](cfg___detail_api_8h.md)

[Go to the documentation of this file](cfg___detail_api_8h.md)


```C++
#pragma once

#include <nn/Handle.h>
#include <nn/Result.h>

namespace nn {
namespace cfg {
namespace CTR {
namespace detail {

typedef enum _IPCPortType
{
        PORT_CFG_USER   = 0,
        PORT_CFG_SYS    = 1,
        PORT_CFG_INIT   = 2,
        PORT_CFG_NOR    = 3,
        NUM_OF_IPC_PORT = 4
} IPCPortType;

Result Initialize();
Result InitializeProperPort(IPCPortType* pPortType);

void Finalize();
void FinalizeProperPort(IPCPortType portType);

Result GetConfig(void* pData, size_t size, bit32 key);

} // namespace detail
} // namespace CTR
} // namespace cfg
} // namespace nn
```


