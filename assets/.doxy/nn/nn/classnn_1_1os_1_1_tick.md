

# Class nn::os::Tick



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**os**](namespacenn_1_1os.md) **>** [**Tick**](classnn_1_1os_1_1_tick.md)





* `#include <os_Tick.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Tick**](#function-tick-12) ([**s64**](types_8h.md#typedef-s64) tick) <br> |
|   | [**Tick**](#function-tick-22) ([**fnd::TimeSpan**](classnn_1_1fnd_1_1_time_span.md) span) <br> |
|  [**fnd::TimeSpan**](classnn_1_1fnd_1_1_time_span.md) | [**ToTimeSpan**](#function-totimespan) () <br> |
|   | [**TimeSpan**](#function-timespan) () <br> |
|   | [**operator s64**](#function-operator-s64) () <br> |
|  [**Tick**](classnn_1_1os_1_1_tick.md) | [**operator-**](#function-operator-) ([**Tick**](classnn_1_1os_1_1_tick.md) rhs) <br> |
|  [**Tick**](classnn_1_1os_1_1_tick.md) & | [**operator-=**](#function-operator-_1) ([**Tick**](classnn_1_1os_1_1_tick.md) rhs) <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**Tick**](classnn_1_1os_1_1_tick.md) | [**GetSystemCurrent**](#function-getsystemcurrent) () <br> |


























## Public Functions Documentation




### function Tick [1/2]

```C++
inline nn::os::Tick::Tick (
    s64 tick
) 
```




<hr>



### function Tick [2/2]

```C++
nn::os::Tick::Tick (
    fnd::TimeSpan span
) 
```




<hr>



### function ToTimeSpan 

```C++
fnd::TimeSpan nn::os::Tick::ToTimeSpan () 
```




<hr>



### function TimeSpan 

```C++
nn::os::Tick::TimeSpan () 
```




<hr>



### function operator s64 

```C++
inline nn::os::Tick::operator s64 () 
```




<hr>



### function operator- 

```C++
inline Tick nn::os::Tick::operator- (
    Tick rhs
) 
```




<hr>



### function operator-= 

```C++
inline Tick & nn::os::Tick::operator-= (
    Tick rhs
) 
```




<hr>
## Public Static Functions Documentation




### function GetSystemCurrent 

```C++
static Tick nn::os::Tick::GetSystemCurrent () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/os/os_Tick.h`

