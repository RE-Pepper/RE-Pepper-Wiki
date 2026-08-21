

# File fs\_UserFileSystem.cpp

[**File List**](files.md) **>** [**CTR**](dir_0db075d501ede26a9de12816de7460c1.md) **>** [**MPCore**](dir_8573f519a3edfd13db8629e441074c88.md) **>** [**fs\_UserFileSystem.cpp**](fs___user_file_system_8cpp.md)

[Go to the documentation of this file](fs___user_file_system_8cpp.md)


```C++
#include <nn/fs/CTR/MPCore/fs_UserFileSystem.h>

RP_SHUTUP

namespace nn {
namespace fs {
namespace CTR {
namespace MPCore {
namespace detail {

namespace {
var(nn::fs::CTR::MPCore::detail, g_FileServerHandle, Handle);
} // namespace

var(nn::fs::CTR::MPCore::detail, s_IsLatencyEmulationEnable, bool) = false;
} // namespace detail
} // namespace MPCore
} // namespace CTR

void ForceDisableLatencyEmulation()
{
        CTR::MPCore::detail::s_IsLatencyEmulationEnable = false;
}

} // namespace fs
} // namespace nn
```


