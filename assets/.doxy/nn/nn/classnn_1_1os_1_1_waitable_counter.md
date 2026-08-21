

# Class nn::os::WaitableCounter



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**os**](namespacenn_1_1os.md) **>** [**WaitableCounter**](classnn_1_1os_1_1_waitable_counter.md)





* `#include <os_WaitableCounter.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**Result**](classnn_1_1_result.md) | [**ArbitrateAddress**](#function-arbitrateaddress) ([**ArbitrationType**](namespacenn_1_1os.md#enum-arbitrationtype) type, [**s32**](types_8h.md#typedef-s32) value) <br> |
|  [**Result**](classnn_1_1_result.md) | [**DecrementAndWaitIfLessThan**](#function-decrementandwaitiflessthan) ([**s32**](types_8h.md#typedef-s32) value) <br> |
|  [**Result**](classnn_1_1_result.md) | [**DecrementAndWaitIfLessThanWithTimeout**](#function-decrementandwaitiflessthanwithtimeout) ([**s32**](types_8h.md#typedef-s32) value) <br> |
|  void | [**Finalize**](#function-finalize) () <br> |
|  void | [**Initialize**](#function-initialize) () <br> |
|  [**Result**](classnn_1_1_result.md) | [**Signal**](#function-signal) ([**s32**](types_8h.md#typedef-s32) value) <br> |
|  [**Result**](classnn_1_1_result.md) | [**SignalAll**](#function-signalall) () <br> |
|  [**Result**](classnn_1_1_result.md) | [**WaitIfLessThan**](#function-waitiflessthan) ([**s32**](types_8h.md#typedef-s32) value) <br> |
|  [**Result**](classnn_1_1_result.md) | [**WaitIfLessThanWithTimeout**](#function-waitiflessthanwithtimeout) ([**s32**](types_8h.md#typedef-s32) value) <br> |
|  [**ValueType**](classnn_1_1os_1_1_waitable_counter.md#typedef-valuetype) & | [**operator\***](#function-operator) () <br> |
|  const [**ValueType**](classnn_1_1os_1_1_waitable_counter.md#typedef-valuetype) & | [**operator\***](#function-operator_1) () const<br> |
|  [**ValueType**](classnn_1_1os_1_1_waitable_counter.md#typedef-valuetype) \* | [**operator-&gt;**](#function-operator-) () <br> |




























## Public Functions Documentation




### function ArbitrateAddress 

```C++
inline Result nn::os::WaitableCounter::ArbitrateAddress (
    ArbitrationType type,
    s32 value
) 
```




<hr>



### function DecrementAndWaitIfLessThan 

```C++
inline Result nn::os::WaitableCounter::DecrementAndWaitIfLessThan (
    s32 value
) 
```




<hr>



### function DecrementAndWaitIfLessThanWithTimeout 

```C++
inline Result nn::os::WaitableCounter::DecrementAndWaitIfLessThanWithTimeout (
    s32 value
) 
```




<hr>



### function Finalize 

```C++
void nn::os::WaitableCounter::Finalize () 
```




<hr>



### function Initialize 

```C++
void nn::os::WaitableCounter::Initialize () 
```




<hr>



### function Signal 

```C++
inline Result nn::os::WaitableCounter::Signal (
    s32 value
) 
```




<hr>



### function SignalAll 

```C++
inline Result nn::os::WaitableCounter::SignalAll () 
```




<hr>



### function WaitIfLessThan 

```C++
inline Result nn::os::WaitableCounter::WaitIfLessThan (
    s32 value
) 
```




<hr>



### function WaitIfLessThanWithTimeout 

```C++
inline Result nn::os::WaitableCounter::WaitIfLessThanWithTimeout (
    s32 value
) 
```




<hr>



### function operator\* 

```C++
inline ValueType & nn::os::WaitableCounter::operator* () 
```




<hr>



### function operator\* 

```C++
inline const ValueType & nn::os::WaitableCounter::operator* () const
```




<hr>



### function operator-&gt; 

```C++
inline ValueType * nn::os::WaitableCounter::operator-> () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/os/os_WaitableCounter.h`

