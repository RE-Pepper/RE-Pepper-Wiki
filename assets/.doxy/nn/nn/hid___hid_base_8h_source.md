

# File hid\_HidBase.h

[**File List**](files.md) **>** [**CTR**](dir_469c329f832ba112fcb0b93bb5878886.md) **>** [**hid\_HidBase.h**](hid___hid_base_8h.md)

[Go to the documentation of this file](hid___hid_base_8h.md)


```C++
#pragma once

#include <nn/os/os_Event.h>

namespace nn {
namespace hid {
namespace CTR {

class HidBase : os::EventBase
{
private:
        uptr m_pResource;

public:
        uptr GetResource () const { return m_pResource; }

        void SetResource (uptr resource)
        {
                this->m_pResource = resource;
        }

        HidBase () {}
        ~HidBase () {}
};
static_assert_ (sizeof (HidBase) == 0x8);

} // namespace CTR
} // namespace hid
} // namespace nn
```


