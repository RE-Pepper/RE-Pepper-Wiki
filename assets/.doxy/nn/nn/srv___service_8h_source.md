

# File srv\_Service.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**srv**](dir_2f77558cefdcdd091fbae5ab2d60e6ab.md) **>** [**srv\_Service.h**](srv___service_8h.md)

[Go to the documentation of this file](srv___service_8h.md)


```C++
#pragma once

#include <nn/Handle.h>
#include <nn/Result.h>

namespace nn {
namespace srv {
namespace detail {

class Service
{
private:
        Handle s_Session;

public:
        static Result RegisterClient ();
        static Result EnableNotification ();
        static Result RegisterService (Handle*, const char8*, s32, s32);
        static Result UnregisterService (const char8*, s32);
        static Result GetServiceHandle (Handle*, const char8*, s32, bit32);
        static Result RegisterObject (Handle, const char8*, s32);
        static Result UnregisterObject (const char8*, s32);
        static Result GetNamedObject (Handle*, const char8*, s32, bool);
        static Result Subscribe (bit32);
        static Result Unsubscribe (bit32);
        static Result PublishToSubscriber (bit32, bit32, bit32);
        static Result IsServiceRegistered (bool*, const char8*, s32);
};

} // namespace detail
} // namespace srv
} // namespace nn
```


