

# File fnd\_DetailHeap.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**fnd**](dir_560a6cc5d6df315094c0d1c837639e89.md) **>** [**detail**](dir_038c443e7cd3fdbb4070ab98702e9044.md) **>** [**fnd\_DetailHeap.h**](fnd___detail_heap_8h.md)

[Go to the documentation of this file](fnd___detail_heap_8h.md)


```C++
#pragma once
#include "./fnd_DetailHeapCommon.h"

namespace nn {
namespace fnd {
namespace detail {

bool IsValidHeapHandle (ConstHeap handle);

void DestroyHeap (Heap heap);

} // namespace detail
} // namespace fnd
} // namespace nn
```


