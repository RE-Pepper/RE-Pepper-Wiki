

# File fnd\_DetailHeapHead.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**fnd**](dir_896b02bd9724af022fac6ecc9927c6e1.md) **>** [**detail**](dir_3da131c86a4fcd1c3423f598aebcaf26.md) **>** [**fnd\_DetailHeapHead.h**](fnd___detail_heap_head_8h.md)

[Go to the documentation of this file](fnd___detail_heap_head_8h.md)


```C++
#pragma once

namespace nn {
namespace fnd {
namespace detail {

typedef struct
{
        void* prevObject;
        void* nextObject;
} NNSFndLink;
static_assert_ (sizeof (NNSFndLink) == 0x8);

typedef struct
{
        void* headObject;
        void* tailObject;
        u16   numObjects;
        u16   offset;
} NNSFndList;
static_assert_ (sizeof (NNSFndList) == 0xC);

struct NNSiFndExpHeapMBlockHead
{
        u16                       signature;
        u16                       attribute;
        u32                       blockSize;
        NNSiFndExpHeapMBlockHead* pMBHeadPrev;
        NNSiFndExpHeapMBlockHead* pMBHeadBext;
};
static_assert_ (sizeof (NNSiFndExpHeapMBlockHead) == 0x10);

struct NNSiFndExpMBlockList
{
        NNSiFndExpHeapMBlockHead* head;
        NNSiFndExpHeapMBlockHead* tail;
};
static_assert_ (sizeof (NNSiFndExpMBlockList) == 0x8);

struct NNSiFndExpHeapHead
{
        NNSiFndExpMBlockList mbFreeList;
        NNSiFndExpMBlockList mbUsedList;
        u16                  groupID;
        u16                  feature;
        bool                 reuse;
        u32 : 24;
};
static_assert_ (sizeof (NNSiFndExpHeapHead) == 0x18);

struct ExpHeapImpl
{
        u32                signature;
        NNSFndLink         link;
        NNSFndList         childList;
        void*              heapStart;
        void*              heapEnd;
        u32                attribute;
        NNSiFndExpHeapHead nnsiFndExpHeapHead;

        ExpHeapImpl () : attribute (0) {}
};
static_assert_ (sizeof (ExpHeapImpl) == 0x3C);

} // namespace detail
} // namespace fnd
} // namespace nn
```


