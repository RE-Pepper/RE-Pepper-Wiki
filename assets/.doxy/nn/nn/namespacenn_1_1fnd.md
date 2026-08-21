

# Namespace nn::fnd



[**Namespace List**](namespaces.md) **>** [**nn**](namespacenn.md) **>** [**fnd**](namespacenn_1_1fnd.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**ARMv6**](namespacenn_1_1fnd_1_1_a_r_mv6.md) <br> |
| namespace | [**detail**](namespacenn_1_1fnd_1_1detail.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**HeapBase**](classnn_1_1fnd_1_1_heap_base.md) <br> |
| class | [**InterlockedVariable**](classnn_1_1fnd_1_1_interlocked_variable.md) &lt;typename T&gt;<br> |
| class | [**IntrusiveLinkedList**](classnn_1_1fnd_1_1_intrusive_linked_list.md) &lt;typename T, typename U&gt;<br> |
| class | [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| enum  | [**Description**](#enum-description)  <br> |
| enum  | [**HeapFillType**](#enum-heapfilltype)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**\_NN\_FND\_RESULT\_DEF\_CONST**](#function-_nn_fnd_result_def_const) (ResultInvalidAddress, LEVEL\_USAGE, SUMMARY\_INVALID\_ARGUMENT, Result::DESCRIPTION\_INVALID\_ADDRESS) <br> |
|   | [**\_NN\_FND\_RESULT\_DEF\_CONST**](#function-_nn_fnd_result_def_const) (ResultFndUnk0, LEVEL\_USAGE, SUMMARY\_INVALID\_ARGUMENT, DESCRIPTION\_UNK2) <br> |




























## Public Types Documentation




### enum Description 

```C++
enum nn::fnd::Description {
    DESCRIPTION_UNK1 = 1,
    DESCRIPTION_UNK2 = 2
};
```




<hr>



### enum HeapFillType 

```C++
enum nn::fnd::HeapFillType {
    HEAP_FILL_TYPE_NOUSE,
    HEAP_FILL_TYPE_ALLOC,
    HEAP_FILL_TYPE_FREE,
    HEAP_FILL_TYPE_MAX
};
```




<hr>
## Public Functions Documentation




### function \_NN\_FND\_RESULT\_DEF\_CONST 

```C++
nn::fnd::_NN_FND_RESULT_DEF_CONST (
    ResultInvalidAddress,
    LEVEL_USAGE,
    SUMMARY_INVALID_ARGUMENT,
    Result::DESCRIPTION_INVALID_ADDRESS
) 
```




<hr>



### function \_NN\_FND\_RESULT\_DEF\_CONST 

```C++
nn::fnd::_NN_FND_RESULT_DEF_CONST (
    ResultFndUnk0,
    LEVEL_USAGE,
    SUMMARY_INVALID_ARGUMENT,
    DESCRIPTION_UNK2
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fnd/ARMv6/fnd_Interlocked.h`

