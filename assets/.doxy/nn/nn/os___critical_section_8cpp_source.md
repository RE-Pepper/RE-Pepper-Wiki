

# File os\_CriticalSection.cpp

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**os**](dir_56153499d95e77076f83f9f8405b15c2.md) **>** [**os\_CriticalSection.cpp**](os___critical_section_8cpp.md)

[Go to the documentation of this file](os___critical_section_8cpp.md)


```C++
#include <nn/os/os_CriticalSection.h>

namespace nn {
namespace os {

void CriticalSection::EnterImpl ()
{
        while (true) {
                if (*m_Counter > 0 && TryEnterImpl ()) {
                        break;
                }

                m_Counter.DecrementAndWaitIfLessThan (0);
        }
}

} // namespace os
} // namespace nn
```


