

# File os\_LightSemaphore.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**os**](dir_53922fdb85244c81a863dd6ad700ec31.md) **>** [**os\_LightSemaphore.h**](os___light_semaphore_8h.md)

[Go to the documentation of this file](os___light_semaphore_8h.md)


```C++
#pragma once

#include <nn/assert.h>
#include <nn/fnd/fnd_Interlocked.h>
#include <nn/os/os_WaitableCounter.h>
#include <nn/util/util_NonCopyable.h>

namespace nn {
namespace os {

class LightSemaphore : util::ADLFireWall::NonCopyable<LightSemaphore>
{
private:
        WaitableCounter               m_Counter;
        fnd::InterlockedVariable<s16> m_NumWaiting;
        s16                           m_Max;

        struct DecrementIfPositive
        {
                bool operator() (s32& x)
                {
                        if (x <= 0) {
                                return false;
                        }
                        return true;
                }
        };
        struct LimitedAdd
        {
                s32 max;
                s32 value;
                s32 beforeUpdate;

                bool operator() (s32& x)
                {
                        beforeUpdate = x;

                        if (x > max - value) {
                                x = max;
                        } else {
                                x += value;
                        }

                        return true;
                }
        };
        static const s32 MAX_MAX_COUNT = 0x7FFF;

public:
        LightSemaphore (s32 initialCount, s32 maxCount)
        {
                Initialize (initialCount, maxCount);
        }
        ~LightSemaphore () {}

        void Initialize (s32 initialCount, s32 maxCount)
        {
                NN_ASSERT_SDK_MIN (initialCount, 0);         // 149
                NN_ASSERT_SDK_MIN (maxCount, 1);             // 150
                NN_ASSERT_SDK_MAX (initialCount, maxCount);  // 151
                NN_ASSERT_SDK_MAX (maxCount, MAX_MAX_COUNT); // 152

                *m_Counter   = initialCount;
                m_NumWaiting = 0;
                m_Max        = maxCount;
        }

        void Initialize (s32 initialCount)
        {
                Initialize (initialCount, MAX_MAX_COUNT);
        }
        s32 GetMax () const { return m_Max; }
        s32 GetCount () const { return *m_Counter; }

        void Acquire ()
        {
                while (!TryAcquire ()) {
                        ++m_NumWaiting;
                        m_Counter.WaitIfLessThan (1);
                        --m_NumWaiting;
                }
        }
        bool TryAcquire ()
        {
                DecrementIfPositive updater;
                return m_Counter->AtomicUpdateConditional (updater);
        }
        s32 Release (s32);
};
static_assert_ (sizeof (LightSemaphore));

} // namespace os
} // namespace nn

#ifdef __cplusplus
extern "C" {
#endif

typedef union nnosLightSemaphore {
} nnosLightSemaphore; //  299

#ifdef __cplusplus
}
#endif
```


