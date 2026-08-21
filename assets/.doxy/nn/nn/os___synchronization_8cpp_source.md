

# File os\_Synchronization.cpp

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**os**](dir_56153499d95e77076f83f9f8405b15c2.md) **>** [**os\_Synchronization.cpp**](os___synchronization_8cpp.md)

[Go to the documentation of this file](os___synchronization_8cpp.md)


```C++
#include <nn/os/os_Synchronization.h>

RP_SHUTUP

namespace nn {
namespace os {

namespace {

struct WaitMultipleObjectsArgs
{
        s32*         pOut;
        WaitObject** objs;
        s32          numHandles;
        bool         waitAll;
        s64*         timeout;
};

Result WaitMultipleImpl (WaitMultipleObjectsArgs* args, Handle* handles)
{
        // TODO
}

void asm (WaitMultipleImplWithAlloca) (WaitMultipleObjectsArgs* args, int, Result (*) (WaitMultipleObjectsArgs*, nn::Handle*))
{
        push  { lr }; // nf
        bics  r3, r1, #1;
        addne r1, r1, #1;
        mov   r3, r1, lsl #2;
        sub   sp, sp, r3;
        mov   r1, sp;
        push { r3 }; // nf
        blx   r2;
        pop { r3 }; // nf
        add   sp, sp, r3;
        pop { pc }; // nf
}
} // namespace

} // namespace os
} // namespace nn
```


