

# Struct nn::fnd::InterlockedVariable::AssignFunc



[**ClassList**](annotated.md) **>** [**AssignFunc**](structnn_1_1fnd_1_1_interlocked_variable_1_1_assign_func.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  T | [**m\_operand**](#variable-m_operand)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AssignFunc**](#function-assignfunc) (const U & operand) <br> |
|  bool | [**operator()**](#function-operator) (T & x) <br> |




























## Public Attributes Documentation




### variable m\_operand 

```C++
T nn::fnd::InterlockedVariable< T >::AssignFunc::m_operand;
```




<hr>
## Public Functions Documentation




### function AssignFunc 

```C++
template<typename U>
inline AssignFunc::AssignFunc (
    const U & operand
) 
```




<hr>



### function operator() 

```C++
inline bool AssignFunc::operator() (
    T & x
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fnd/fnd_Interlocked.h`

