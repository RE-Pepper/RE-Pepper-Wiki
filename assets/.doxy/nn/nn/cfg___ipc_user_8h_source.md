

# File cfg\_IpcUser.h

[**File List**](files.md) **>** [**cfg**](dir_d61dd7901f361aace8efbc35eb1e8191.md) **>** [**CTR**](dir_6286be2e3839b9d14dbaf851f98cbdb4.md) **>** [**cfg\_IpcUser.h**](cfg___ipc_user_8h.md)

[Go to the documentation of this file](cfg___ipc_user_8h.md)


```C++
#pragma once

#include <nn/Handle.h>
#include <nn/Result.h>
#include <nn/cfg/CTR/cfg_RegionCode.h>

namespace nn {
namespace cfg {
namespace CTR {
namespace detail {

class IpcUser
{
private:
        Handle s_Session;

public:
        Result GetConfig (void* pData, size_t size, bit32 key) const;
        Result GetRegion (CfgRegionCode*) const;
        Result GetTransferableId (bit32, bit64*);
        Result IsCoppacsSupported (bool*);
};
static_assert_ (sizeof (IpcUser) == 4);

} // namespace detail
} // namespace CTR
} // namespace cfg
} // namespace nn
```


