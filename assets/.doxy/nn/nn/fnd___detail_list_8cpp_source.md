

# File fnd\_DetailList.cpp

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**fnd**](dir_560a6cc5d6df315094c0d1c837639e89.md) **>** [**detail**](dir_038c443e7cd3fdbb4070ab98702e9044.md) **>** [**fnd\_DetailList.cpp**](fnd___detail_list_8cpp.md)

[Go to the documentation of this file](fnd___detail_list_8cpp.md)


```C++
#pragma once

#include "./fnd_DetailList.h"

#include <nn/assert.h>

namespace nn {
namespace fnd {
namespace detail {

void RemoveListObject (NNSFndList* list, void* object) // 196
{
        NN_ASSERT_SDK (list);   // 200
        NN_ASSERT_SDK (object); // 201

        NNSFndLink* link = (NNSFndLink*)((u32)object + list->offset);
        if (link->prevObject == NULL) {
                list->headObject = link->nextObject;
        } else {
                ((NNSFndLink*)((u32)link->prevObject + list->offset))->nextObject = link->nextObject;
        }
        if (link->nextObject == NULL) {
                list->tailObject = link->prevObject;
        } else {
                ((NNSFndLink*)((u32)link->nextObject + list->offset))->prevObject = link->prevObject;
        }

        link->nextObject = link->prevObject = NULL;
        --list->numObjects;
}

void* GetNextListObject (const NNSFndList* list, const void* object) // 240
{
        NN_ASSERT_SDK (list); // 242
        if (object == NULL) {
                return list->headObject;
        }
        return ((NNSFndLink*)(u32)object + list->offset)->nextObject;
}

} // namespace detail
} // namespace fnd
} // namespace nn
```


