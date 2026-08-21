

# File os\_WaitableCounter.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**os**](dir_53922fdb85244c81a863dd6ad700ec31.md) **>** [**os\_WaitableCounter.h**](os___waitable_counter_8h.md)

[Go to the documentation of this file](os___waitable_counter_8h.md)


```C++
#pragma once

#include <nn/Handle.h>
#include <nn/Result.h>
#include <nn/fnd/fnd_Interlocked.h>
#include <nn/os/os_Types.h>
#include <nn/svc/svc_Stub.h>

namespace nn {
namespace os {
class WaitableCounter
{
        static nnHandle s_Handle;

private:
        typedef fnd::InterlockedVariable<s32> ValueType; // 36
        ValueType                             m_Value;

public:
        void Initialize ();
        void Finalize ();

        ValueType&       operator* () { return m_Value; }
        const ValueType& operator* () const { return m_Value; }
        ValueType*       operator->() { return &m_Value; }

        Result ArbitrateAddress (ArbitrationType type, s32 value)
        {
                return svc::ArbitrateAddress (s_Handle, (uptr)&m_Value, type, value);
        }
        Result WaitIfLessThan (s32 value)
        {
                return ArbitrateAddress (ARBITRATION_TYPE_WAIT_IF_LESS_THAN, value);
        }
        Result WaitIfLessThanWithTimeout (s32 value)
        {
                return ArbitrateAddress (ARBITRATION_TYPE_WAIT_IF_LESS_THAN_WITH_TIMEOUT, value);
        }
        Result DecrementAndWaitIfLessThan (s32 value)
        {
                return ArbitrateAddress (ARBITRATION_TYPE_DECREMENT_AND_WAIT_IF_LESS_THAN, value);
        }
        Result DecrementAndWaitIfLessThanWithTimeout (s32 value)
        {
                return ArbitrateAddress (ARBITRATION_TYPE_DECREMENT_AND_WAIT_IF_LESS_THAN_WITH_TIMEOUT, value);
        }
        Result Signal (s32 value)
        {
                return ArbitrateAddress (ARBITRATION_TYPE_SIGNAL, value);
        }
        Result SignalAll ()
        {
                return Signal (-1);
        }
};

} // namespace os
} // namespace nn
```


