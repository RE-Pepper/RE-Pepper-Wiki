

# Class nn::fnd::HeapBase



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fnd**](namespacenn_1_1fnd.md) **>** [**HeapBase**](classnn_1_1fnd_1_1_heap_base.md)





* `#include <fnd_HeapBase.h>`



Inherits the following classes: [nn::fnd::IntrusiveLinkedList::Item](classnn_1_1fnd_1_1_intrusive_linked_list_1_1_item.md)










































































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**DebugFillMemory**](#function-debugfillmemory) ([**uptr**](types_8h.md#typedef-uptr), size\_t, [**HeapFillType**](namespacenn_1_1fnd.md#enum-heapfilltype)) <br> |
|  void | [**Destroy**](#function-destroy) ([**HeapBase**](classnn_1_1fnd_1_1_heap_base.md) \*) <br> |
|  void | [**FillMemoryZero**](#function-fillmemoryzero) ([**uptr**](types_8h.md#typedef-uptr), size\_t size) <br> |
|  [**HeapBase**](classnn_1_1fnd_1_1_heap_base.md) \* | [**FindHeap**](#function-findheap) (void \*) <br> |
|  [**u32**](types_8h.md#typedef-u32) | [**GetFillValue**](#function-getfillvalue) ([**HeapFillType**](namespacenn_1_1fnd.md#enum-heapfilltype)) <br> |
|  [**HeapBase**](classnn_1_1fnd_1_1_heap_base.md) \* | [**GetRoot**](#function-getroot) () <br> |
|  void | [**Initialize**](#function-initialize) ([**bit32**](types_8h.md#typedef-bit32) option) <br> |
|  void | [**SetParent**](#function-setparent) ([**HeapBase**](classnn_1_1fnd_1_1_heap_base.md) \*) <br> |
|   | [**~HeapBase**](#function-heapbase) () <br> |


## Public Functions inherited from nn::fnd::IntrusiveLinkedList::Item

See [nn::fnd::IntrusiveLinkedList::Item](classnn_1_1fnd_1_1_intrusive_linked_list_1_1_item.md)

| Type | Name |
| ---: | :--- |
|   | [**Item**](classnn_1_1fnd_1_1_intrusive_linked_list_1_1_item.md#function-item) () <br> |
|   | [**~Item**](classnn_1_1fnd_1_1_intrusive_linked_list_1_1_item.md#function-item) () <br> |




## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**FillMemory**](#function-fillmemory) ([**uptr**](types_8h.md#typedef-uptr), [**uptr**](types_8h.md#typedef-uptr), [**bit8**](types_8h.md#typedef-bit8)) <br> |
|  void | [**FillMemory32**](#function-fillmemory32) ([**uptr**](types_8h.md#typedef-uptr), [**uptr**](types_8h.md#typedef-uptr), [**bit8**](types_8h.md#typedef-bit8)) <br> |
|  [**uptr**](types_8h.md#typedef-uptr) | [**RoundDown**](#function-rounddown) ([**uptr**](types_8h.md#typedef-uptr), [**s32**](types_8h.md#typedef-s32)) <br> |
|  [**uptr**](types_8h.md#typedef-uptr) | [**RoundUp**](#function-roundup) ([**uptr**](types_8h.md#typedef-uptr), [**s32**](types_8h.md#typedef-s32)) <br> |






































































## Protected Functions inherited from nn::util::ADLFireWall::NonCopyable

See [nn::util::ADLFireWall::NonCopyable](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md)

| Type | Name |
| ---: | :--- |
|   | [**NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable-12) () <br> |
|   | [**~NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable) () <br> |








## Public Functions Documentation




### function DebugFillMemory 

```C++
inline void nn::fnd::HeapBase::DebugFillMemory (
    uptr,
    size_t,
    HeapFillType
) 
```




<hr>



### function Destroy 

```C++
void nn::fnd::HeapBase::Destroy (
    HeapBase *
) 
```




<hr>



### function FillMemoryZero 

```C++
void nn::fnd::HeapBase::FillMemoryZero (
    uptr,
    size_t size
) 
```




<hr>



### function FindHeap 

```C++
HeapBase * nn::fnd::HeapBase::FindHeap (
    void *
) 
```




<hr>



### function GetFillValue 

```C++
u32 nn::fnd::HeapBase::GetFillValue (
    HeapFillType
) 
```




<hr>



### function GetRoot 

```C++
HeapBase * nn::fnd::HeapBase::GetRoot () 
```




<hr>



### function Initialize 

```C++
void nn::fnd::HeapBase::Initialize (
    bit32 option
) 
```




<hr>



### function SetParent 

```C++
void nn::fnd::HeapBase::SetParent (
    HeapBase *
) 
```




<hr>



### function ~HeapBase 

```C++
nn::fnd::HeapBase::~HeapBase () 
```




<hr>
## Public Static Functions Documentation




### function FillMemory 

```C++
static void nn::fnd::HeapBase::FillMemory (
    uptr,
    uptr,
    bit8
) 
```




<hr>



### function FillMemory32 

```C++
static void nn::fnd::HeapBase::FillMemory32 (
    uptr,
    uptr,
    bit8
) 
```




<hr>



### function RoundDown 

```C++
static uptr nn::fnd::HeapBase::RoundDown (
    uptr,
    s32
) 
```




<hr>



### function RoundUp 

```C++
static uptr nn::fnd::HeapBase::RoundUp (
    uptr,
    s32
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fnd/fnd_HeapBase.h`

