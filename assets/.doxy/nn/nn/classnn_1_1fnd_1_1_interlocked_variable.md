

# Class nn::fnd::InterlockedVariable

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fnd**](namespacenn_1_1fnd.md) **>** [**InterlockedVariable**](classnn_1_1fnd_1_1_interlocked_variable.md)





* `#include <fnd_Interlocked.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|  bool | [**AtomicUpdateConditional**](#function-atomicupdateconditional) (UpdateFunc & func) <br> |
|  T | [**CompareAndSwap**](#function-compareandswap) (T comprand, T value) <br> |
|   | [**InterlockedVariable**](#function-interlockedvariable) () <br> |
|   | [**operator T**](#function-operator-t) () const<br> |
|  void | [**operator++**](#function-operator) () <br> |
|  void | [**operator--**](#function-operator-) () <br> |
|  void | [**operator=**](#function-operator_1) (U value) <br> |




























## Public Functions Documentation




### function AtomicUpdateConditional 

```C++
template<typename UpdateFunc>
inline bool nn::fnd::InterlockedVariable::AtomicUpdateConditional (
    UpdateFunc & func
) 
```




<hr>



### function CompareAndSwap 

```C++
inline T nn::fnd::InterlockedVariable::CompareAndSwap (
    T comprand,
    T value
) 
```




<hr>



### function InterlockedVariable 

```C++
inline nn::fnd::InterlockedVariable::InterlockedVariable () 
```




<hr>



### function operator T 

```C++
inline nn::fnd::InterlockedVariable::operator T () const
```




<hr>



### function operator++ 

```C++
inline void nn::fnd::InterlockedVariable::operator++ () 
```




<hr>



### function operator-- 

```C++
inline void nn::fnd::InterlockedVariable::operator-- () 
```




<hr>



### function operator= 

```C++
template<typename U>
inline void nn::fnd::InterlockedVariable::operator= (
    U value
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fnd/fnd_Interlocked.h`

