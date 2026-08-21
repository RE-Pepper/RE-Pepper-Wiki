

# File os\_Event.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**os**](dir_53922fdb85244c81a863dd6ad700ec31.md) **>** [**os\_Event.h**](os___event_8h.md)

[Go to the documentation of this file](os___event_8h.md)


```C++
#pragma once

#include <nn/os/os_Synchronization.h>
#include <nn/os/os_Types.h>

#include "nn/fnd/fnd_TimeSpan.h"
#include "nn/os/CTR/os_ErrorHandler.h"
#include "nn/svc/svc_Stub.h"

namespace nn {
namespace os {

class EventBase : public InterruptEvent
{
public:
        EventBase ()
        {
        }
        EventBase (ResetType resetType)
        {
                Initialize (resetType);
        }
        ~EventBase ()
        {
        }

        Result TryInitialize (ResetType resetType)
        {
                Result result = TryInitializeImpl (resetType);
                if (result.GetSummary () == Result::SUMMARY_OUT_OF_RESOURCE) {
                        return result;
                }
                NN_OS_HANDLE_ERROR (result);
                return result;
        }
        void Initialize (ResetType resetType)
        {
                NN_OS_HANDLE_ERROR (TryInitialize (resetType));
        }
        void Signal ()
        {
                NN_OS_HANDLE_ERROR (svc::SignalEvent (GetHandle ()));
        }
        void ClearSignal ()
        {
                NN_OS_HANDLE_ERROR (svc::ClearEvent (GetHandle ()));
        }
        Result TryInitializeImpl (ResetType resetType)
        {
                Handle handle;
                Result nn_util_return_if_failure_result;
                // TODO
        }
};
static_assert_ (sizeof (EventBase) == 0x4);

class Event : public EventBase
{
public:
        Event () {}

        Result TryInitialize () { return EventBase::TryInitialize (); }
        void   Initialize (ResetType manualReset) { EventBase::Initialize (manualReset); }

        ~Event () {}

        void Signal () { EventBase::Signal (); }
        void ClearSignal () { EventBase::ClearSignal (); }
        void Wait (fnd::TimeSpan timeout) { WaitOne (timeout); }
};
static_assert_ (sizeof (Event) == 0x4);

} // namespace os
} // namespace nn

#ifdef __cplusplus
extern "C" {
#endif

typedef union nnosEvent {
} nnosEvent;

// nnos..(); come here

#ifdef __cplusplus
}
#endif

```


