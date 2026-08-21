

# File os\_LightSemaphore.cpp

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**os**](dir_56153499d95e77076f83f9f8405b15c2.md) **>** [**os\_LightSemaphore.cpp**](os___light_semaphore_8cpp.md)

[Go to the documentation of this file](os___light_semaphore_8cpp.md)


```C++
#include <nn/os/os_LightSemaphore.h>

#include "nn/assert.h"

namespace nn {
namespace os {

RP_SHUTUP

s32 LightSemaphore::Release (s32 releaseCount)
{
        NN_ASSERT_SDK_MAX (releaseCount, 1); // 24
        // TODO
}

} // namespace os
} // namespace nn
```


