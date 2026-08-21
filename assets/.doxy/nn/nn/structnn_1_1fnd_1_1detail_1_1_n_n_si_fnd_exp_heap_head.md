

# Struct nn::fnd::detail::NNSiFndExpHeapHead



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fnd**](namespacenn_1_1fnd.md) **>** [**detail**](namespacenn_1_1fnd_1_1detail.md) **>** [**NNSiFndExpHeapHead**](structnn_1_1fnd_1_1detail_1_1_n_n_si_fnd_exp_heap_head.md)





* `#include <fnd_DetailHeapHead.h>`





















## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**u32**](types_8h.md#typedef-u32) | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
|  [**u16**](types_8h.md#typedef-u16) | [**feature**](#variable-feature)  <br> |
|  [**u16**](types_8h.md#typedef-u16) | [**groupID**](#variable-groupid)  <br> |
|  [**NNSiFndExpMBlockList**](structnn_1_1fnd_1_1detail_1_1_n_n_si_fnd_exp_m_block_list.md) | [**mbFreeList**](#variable-mbfreelist)  <br> |
|  [**NNSiFndExpMBlockList**](structnn_1_1fnd_1_1detail_1_1_n_n_si_fnd_exp_m_block_list.md) | [**mbUsedList**](#variable-mbusedlist)  <br> |
|  bool | [**reuse**](#variable-reuse)  <br> |












































## Public Attributes Documentation




### variable \_\_pad0\_\_ 

```C++
u32 nn::fnd::detail::NNSiFndExpHeapHead::__pad0__;
```




<hr>



### variable feature 

```C++
u16 nn::fnd::detail::NNSiFndExpHeapHead::feature;
```




<hr>



### variable groupID 

```C++
u16 nn::fnd::detail::NNSiFndExpHeapHead::groupID;
```




<hr>



### variable mbFreeList 

```C++
NNSiFndExpMBlockList nn::fnd::detail::NNSiFndExpHeapHead::mbFreeList;
```




<hr>



### variable mbUsedList 

```C++
NNSiFndExpMBlockList nn::fnd::detail::NNSiFndExpHeapHead::mbUsedList;
```




<hr>



### variable reuse 

```C++
bool nn::fnd::detail::NNSiFndExpHeapHead::reuse;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fnd/detail/fnd_DetailHeapHead.h`

