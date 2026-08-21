

# Namespace nn::fnd::detail



[**Namespace List**](namespaces.md) **>** [**nn**](namespacenn.md) **>** [**fnd**](namespacenn_1_1fnd.md) **>** [**detail**](namespacenn_1_1fnd_1_1detail.md)




















## Classes

| Type | Name |
| ---: | :--- |
| struct | [**ExpHeapImpl**](structnn_1_1fnd_1_1detail_1_1_exp_heap_impl.md) <br> |
| struct | [**NNSFndLink**](structnn_1_1fnd_1_1detail_1_1_n_n_s_fnd_link.md) <br> |
| struct | [**NNSFndList**](structnn_1_1fnd_1_1detail_1_1_n_n_s_fnd_list.md) <br> |
| struct | [**NNSiFndExpHeapHead**](structnn_1_1fnd_1_1detail_1_1_n_n_si_fnd_exp_heap_head.md) <br> |
| struct | [**NNSiFndExpHeapMBlockHead**](structnn_1_1fnd_1_1detail_1_1_n_n_si_fnd_exp_heap_m_block_head.md) <br> |
| struct | [**NNSiFndExpMBlockList**](structnn_1_1fnd_1_1detail_1_1_n_n_si_fnd_exp_m_block_list.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**NNSiFndHeapHead**](namespacenn_1_1fnd_1_1detail.md#typedef-nnsifndheaphead) const  \* | [**ConstHeap**](#typedef-constheap)  <br> |
| typedef [**NNSiFndHeapHead**](namespacenn_1_1fnd_1_1detail.md#typedef-nnsifndheaphead) \* | [**Heap**](#typedef-heap)  <br> |
| typedef [**ExpHeapImpl**](structnn_1_1fnd_1_1detail_1_1_exp_heap_impl.md) | [**NNSiFndHeapHead**](#typedef-nnsifndheaphead)  <br> |
| typedef [**u32**](types_8h.md#typedef-u32) | [**NNSiUIntPtr**](#typedef-nnsiuintptr)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**DestroyHeap**](#function-destroyheap) ([**Heap**](namespacenn_1_1fnd_1_1detail.md#typedef-heap) heap) <br> |
|  void | [**DumpHeapList**](#function-dumpheaplist) () <br> |
|  [**NNSiFndHeapHead**](namespacenn_1_1fnd_1_1detail.md#typedef-nnsifndheaphead) \* | [**FindContainHeap**](#function-findcontainheap) ([**NNSFndList**](structnn_1_1fnd_1_1detail_1_1_n_n_s_fnd_list.md) \* pList, const void \* memBlock) <br> |
|  [**NNSFndList**](structnn_1_1fnd_1_1detail_1_1_n_n_s_fnd_list.md) \* | [**FindListContainHeap**](#function-findlistcontainheap) ([**NNSiFndHeapHead**](namespacenn_1_1fnd_1_1detail.md#typedef-nnsifndheaphead) \* pHeapHd) <br> |
|  [**u32**](types_8h.md#typedef-u32) | [**GetFillValForHeap**](#function-getfillvalforheap) (int type) <br> |
|  void \* | [**GetNextListObject**](#function-getnextlistobject) (const [**NNSFndList**](structnn_1_1fnd_1_1detail_1_1_n_n_s_fnd_list.md) \* list, const void \* object) <br> |
|  bool | [**IsValidHeapHandle**](#function-isvalidheaphandle) ([**ConstHeap**](namespacenn_1_1fnd_1_1detail.md#typedef-constheap) handle) <br> |
|  [**NNSiUIntPtr**](namespacenn_1_1fnd_1_1detail.md#typedef-nnsiuintptr) | [**NNSiGetUIntPtr**](#function-nnsigetuintptr) (const void \* ptr) <br> |
|  void | [**NNSi\_FndFinalizeHeap**](#function-nnsi_fndfinalizeheap) ([**NNSiFndHeapHead**](namespacenn_1_1fnd_1_1detail.md#typedef-nnsifndheaphead) \* pHeapHd) <br> |
|  void | [**RemoveListObject**](#function-removelistobject) ([**NNSFndList**](structnn_1_1fnd_1_1detail_1_1_n_n_s_fnd_list.md) \* list, void \* object) <br> |
|   | [**var**](#function-var) (nn::fnd::detail, sRootList, [**NNSFndList**](structnn_1_1fnd_1_1detail_1_1_n_n_s_fnd_list.md)) <br> |
|   | [**var**](#function-var) (nn::fnd::detail, sRootListInitialized, bool) <br> |
|   | [**var**](#function-var) (nn::fnd::detail, sFillVals, [**u32**](types_8h.md#typedef-u32)) <br> |




























## Public Types Documentation




### typedef ConstHeap 

```C++
typedef NNSiFndHeapHead const* nn::fnd::detail::ConstHeap;
```




<hr>



### typedef Heap 

```C++
typedef NNSiFndHeapHead* nn::fnd::detail::Heap;
```




<hr>



### typedef NNSiFndHeapHead 

```C++
typedef ExpHeapImpl nn::fnd::detail::NNSiFndHeapHead;
```




<hr>



### typedef NNSiUIntPtr 

```C++
typedef u32 nn::fnd::detail::NNSiUIntPtr;
```




<hr>
## Public Functions Documentation




### function DestroyHeap 

```C++
void nn::fnd::detail::DestroyHeap (
    Heap heap
) 
```




<hr>



### function DumpHeapList 

```C++
void nn::fnd::detail::DumpHeapList () 
```




<hr>



### function FindContainHeap 

```C++
NNSiFndHeapHead * nn::fnd::detail::FindContainHeap (
    NNSFndList * pList,
    const void * memBlock
) 
```




<hr>



### function FindListContainHeap 

```C++
NNSFndList * nn::fnd::detail::FindListContainHeap (
    NNSiFndHeapHead * pHeapHd
) 
```




<hr>



### function GetFillValForHeap 

```C++
u32 nn::fnd::detail::GetFillValForHeap (
    int type
) 
```




<hr>



### function GetNextListObject 

```C++
void * nn::fnd::detail::GetNextListObject (
    const NNSFndList * list,
    const void * object
) 
```




<hr>



### function IsValidHeapHandle 

```C++
bool nn::fnd::detail::IsValidHeapHandle (
    ConstHeap handle
) 
```




<hr>



### function NNSiGetUIntPtr 

```C++
NNSiUIntPtr nn::fnd::detail::NNSiGetUIntPtr (
    const void * ptr
) 
```




<hr>



### function NNSi\_FndFinalizeHeap 

```C++
void nn::fnd::detail::NNSi_FndFinalizeHeap (
    NNSiFndHeapHead * pHeapHd
) 
```




<hr>



### function RemoveListObject 

```C++
void nn::fnd::detail::RemoveListObject (
    NNSFndList * list,
    void * object
) 
```




<hr>



### function var 

```C++
nn::fnd::detail::var (
    nn::fnd::detail,
    sRootList,
    NNSFndList
) 
```




<hr>



### function var 

```C++
nn::fnd::detail::var (
    nn::fnd::detail,
    sRootListInitialized,
    bool
) 
```




<hr>



### function var 

```C++
nn::fnd::detail::var (
    nn::fnd::detail,
    sFillVals,
    u32
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fnd/detail/fnd_DetailHeapHead.h`

