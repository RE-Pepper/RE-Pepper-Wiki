

# File util\_NonCopyable.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**util**](dir_369320240f3428c6f0d988f9f85aef22.md) **>** [**util\_NonCopyable.h**](util___non_copyable_8h.md)

[Go to the documentation of this file](util___non_copyable_8h.md)


```C++
#pragma once

namespace nn {
namespace util {
namespace ADLFireWall {

template <typename T>
struct NonCopyable
{
protected:
        NonCopyable () {}
        ~NonCopyable () {}

private:
        NonCopyable (const NonCopyable&);
};

} // namespace ADLFireWall
} // namespace util
} // namespace nn
```


