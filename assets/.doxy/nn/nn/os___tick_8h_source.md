

# File os\_Tick.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**os**](dir_53922fdb85244c81a863dd6ad700ec31.md) **>** [**os\_Tick.h**](os___tick_8h.md)

[Go to the documentation of this file](os___tick_8h.md)


```C++
#pragma once

#include <nn/fnd/fnd_TimeSpan.h>

#include "nn/svc/svc_Stub.h"

namespace nn {
namespace os {

class Tick
{
private:
        s64 m_Tick;

public:
        Tick (s64 tick) : m_Tick (tick) {} // 51
        Tick (fnd::TimeSpan span);         // 109

        operator s64 () { return m_Tick; } // 63
        operator fnd::TimeSpan ();         // 113

        fnd::TimeSpan ToTimeSpan (); // 118

        static Tick GetSystemCurrent (); // 104

        Tick& operator-= (Tick rhs) { this->m_Tick -= rhs.m_Tick; } // 89
        Tick  operator- (Tick rhs) {}                               // 90
};

Tick Tick::GetSystemCurrent () // 104
{
        return Tick (svc::GetSystemTick ());
}

Tick::Tick (fnd::TimeSpan span) // 109
{
        // TODO
}
Tick::operator fnd::TimeSpan () // 113
{
        // TODO
}

fnd::TimeSpan Tick::ToTimeSpan () // 118
{
        // TODO
}

} // namespace os
} // namespace nn
```


