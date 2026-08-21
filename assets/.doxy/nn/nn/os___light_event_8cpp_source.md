

# File os\_LightEvent.cpp

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**os**](dir_56153499d95e77076f83f9f8405b15c2.md) **>** [**os\_LightEvent.cpp**](os___light_event_8cpp.md)

[Go to the documentation of this file](os___light_event_8cpp.md)


```C++
#include <nn/os/os_LightEvent.h>

RP_SHUTUP

namespace nn {
namespace os {

bool LightEvent::TryWait ()
{ // 32
        if (*m_Counter == RESET_UNK1) {
                return true;
        }

        return m_Counter->CompareAndSwap (RESET_UNK0, RESET_AUTO) == RESET_UNK0;
}

void LightEvent::Wait ()
{ // 102
        while (true) {
                switch (*m_Counter) {
                case RESET_MANUAL:
                        m_Counter.WaitIfLessThan (0);
                        return;
                case RESET_UNK1:
                        return;
                case RESET_AUTO:
                        break;
                case RESET_UNK0:
                        if (m_Counter->CompareAndSwap (RESET_UNK0, RESET_AUTO) == RESET_UNK0) {
                                return;
                        }
                        break;
                }

                m_Counter.WaitIfLessThan (0);
        }
}

void LightEvent::Signal ()
{ // 135
        if (*m_Counter == RESET_AUTO) {
                *m_Counter = RESET_UNK0;
                m_Counter.Signal (1);
        } else if (*m_Counter == RESET_MANUAL) {
                *m_Counter = RESET_UNK1;
                m_Counter.SignalAll ();
        }
}

void LightEvent::Pulse ()
{
        // UNUSED
}

void LightEvent::ClearSignal ()
{ // 189
        if (*m_Counter == RESET_UNK1) {
                *m_Counter = RESET_AUTO;
        } else if (*m_Counter == RESET_UNK0) {
                *m_Counter = RESET_MANUAL;
        }
}

} // namespace os
} // namespace nn
```


