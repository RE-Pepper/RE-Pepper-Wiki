

# File fnd\_DetailHeapCommon.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**fnd**](dir_560a6cc5d6df315094c0d1c837639e89.md) **>** [**detail**](dir_038c443e7cd3fdbb4070ab98702e9044.md) **>** [**fnd\_DetailHeapCommon.h**](fnd___detail_heap_common_8h.md)

[Go to the documentation of this file](fnd___detail_heap_common_8h.md)


```C++
#pragma once

#include <nn/fnd/detail/fnd_DetailHeapHead.h>

namespace nn {
namespace fnd {
namespace detail {

typedef ExpHeapImpl            NNSiFndHeapHead; // 96
typedef NNSiFndHeapHead*       Heap;            // 97
typedef NNSiFndHeapHead const* ConstHeap;       // 98

NNSiFndHeapHead* FindContainHeap (NNSFndList* pList, const void* memBlock);
NNSFndList*      FindListContainHeap (NNSiFndHeapHead* pHeapHd);
void             DumpHeapList ();
void             NNSi_FndFinalizeHeap (NNSiFndHeapHead* pHeapHd);
u32              GetFillValForHeap (int type);

#define NN_HEAP_EXP_IDENT 0x45585048 // b'EXPH'

} // namespace detail
} // namespace fnd
} // namespace nn
```


