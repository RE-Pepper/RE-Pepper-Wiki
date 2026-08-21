

# File srv\_Api.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**srv**](dir_2f77558cefdcdd091fbae5ab2d60e6ab.md) **>** [**srv\_Api.h**](srv___api_8h.md)

[Go to the documentation of this file](srv___api_8h.md)


```C++
#pragma once

#include <nn/Handle.h>
#include <nn/Result.h>
#include <nn/fnd/fnd_LinkedList.h>
#include <nn/os/os_LightEvent.h>

namespace nn {
namespace srv {

template <class T>
class EventNotificationHandlerBase
{
private:
        os::LightEvent* m_pEvent;

public:
        EventNotificationHandlerBase () {}

        void Initialize (os::LightEvent* event) {}

        virtual void v0 ();
        virtual void v1 ();
        virtual void v2 ();
        virtual void v3 ();
        virtual void v4 ();
        virtual void v5 ();
        virtual void HandleNotification (bit32) {}
};

class NotificationHandler : public nn::fnd::IntrusiveLinkedList<NotificationHandler>::Item
{
private:
        bit32 m_AttachedMessage;

public:
        NotificationHandler () {}
};

typedef EventNotificationHandlerBase<NotificationHandler*> LightEventNotificationHandler; // 122

Result Initialize ();
Result GetServiceHandle (Handle* pOut, const char8* pName, s32 length, bit32 flags);

inline Result ReceiveNotification (bit32 pOut) // 265
{
        // TODO
}
inline Result GetServiceHandle (Handle* pOut, const char8* pName) // 308
{
        s32 length;
        // TODO
}
inline Result TryGetServiceHandle (Handle* pOut, const char8* pName) // 319
{
        s32 length;
        // TODO
}

} // namespace srv
} // namespace nn
```


