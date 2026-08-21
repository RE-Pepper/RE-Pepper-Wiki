

# Struct nn::fnd::InterlockedVariable::CompareAndSwapFunc



[**ClassList**](annotated.md) **>** [**CompareAndSwapFunc**](structnn_1_1fnd_1_1_interlocked_variable_1_1_compare_and_swap_func.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  T | [**m\_comparand**](#variable-m_comparand)  <br> |
|  T | [**m\_result**](#variable-m_result)  <br> |
|  T | [**m\_value**](#variable-m_value)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**CompareAndSwapFunc**](#function-compareandswapfunc) (T comparand, T value) <br> |
|  bool | [**operator()**](#function-operator) (T & x) <br> |




























## Public Attributes Documentation




### variable m\_comparand 

```C++
T nn::fnd::InterlockedVariable< T >::CompareAndSwapFunc::m_comparand;
```




<hr>



### variable m\_result 

```C++
T nn::fnd::InterlockedVariable< T >::CompareAndSwapFunc::m_result;
```




<hr>



### variable m\_value 

```C++
T nn::fnd::InterlockedVariable< T >::CompareAndSwapFunc::m_value;
```




<hr>
## Public Functions Documentation




### function CompareAndSwapFunc 

```C++
inline CompareAndSwapFunc::CompareAndSwapFunc (
    T comparand,
    T value
) 
```




<hr>



### function operator() 

```C++
inline bool CompareAndSwapFunc::operator() (
    T & x
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fnd/fnd_Interlocked.h`

