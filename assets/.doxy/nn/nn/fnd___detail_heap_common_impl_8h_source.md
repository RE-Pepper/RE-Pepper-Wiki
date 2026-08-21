

# File fnd\_DetailHeapCommonImpl.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**fnd**](dir_560a6cc5d6df315094c0d1c837639e89.md) **>** [**detail**](dir_038c443e7cd3fdbb4070ab98702e9044.md) **>** [**fnd\_DetailHeapCommonImpl.h**](fnd___detail_heap_common_impl_8h.md)

[Go to the documentation of this file](fnd___detail_heap_common_impl_8h.md)


```C++
#pragma once

namespace nn {
namespace fnd {
namespace detail {

typedef u32 NNSiUIntPtr;

NNSiUIntPtr NNSiGetUIntPtr (const void* ptr)
{
        return NNSiUIntPtr (ptr);
}

} // namespace detail
} // namespace fnd
} // namespace nn
```


