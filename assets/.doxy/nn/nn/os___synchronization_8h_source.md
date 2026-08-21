

# File os\_Synchronization.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**os**](dir_53922fdb85244c81a863dd6ad700ec31.md) **>** [**os\_Synchronization.h**](os___synchronization_8h.md)

[Go to the documentation of this file](os___synchronization_8h.md)


```C++
#pragma once

#include <nn/Result.h>
#include <nn/fnd/fnd_TimeSpan.h>
#include <nn/os/CTR/os_ErrorHandler.h>
#include <nn/os/os_HandleObject.h>
#include <nn/svc/svc_Inlines.h>

namespace nn {
namespace os {

class WaitObject : public HandleObject
{
private:
        static Result WaitMultiple (s32* pOut, WaitObject** objs, s32 numHandles, bool waitAll, s64 timeout);

public:
        Result WaitOneImpl (s64 nanoSecondsTimeout)
        {
                Handle handle = GetHandle ();
                s32    dummy;
                return svc::WaitSynchronization (&dummy, &handle, 1, 0, nanoSecondsTimeout);
        }
        void WaitOne ()
        {
                NN_OS_HANDLE_ERROR (WaitOneImpl (-1));
        }
        bool WaitOne (fnd::TimeSpan timeout)
        {
                Result result = WaitOneImpl (timeout.GetNanoSeconds ());

                NN_OS_HANDLE_ERROR (result);

                return result.GetDescription () != Result::DESCRIPTION_TIMEOUT;
        }
        static s32 WaitAny (WaitObject** objs, s32 numObjects)
        {
                s32 ret;

                NN_OS_HANDLE_ERROR (WaitMultiple (&ret, objs, numObjects, false, -1));

                return ret;
        }

        WaitObject () {}
        ~WaitObject () {}
};

class InterruptEvent : public WaitObject
{
public:
        InterruptEvent () {}
        ~InterruptEvent () {}
};

} // namespace os
} // namespace nn
```


