

# Class nn::os::LightEvent



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**os**](namespacenn_1_1os.md) **>** [**LightEvent**](classnn_1_1os_1_1_light_event.md)





* `#include <os_LightEvent.h>`



Inherits the following classes: [nn::util::ADLFireWall::NonCopyable](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**ClearSignal**](#function-clearsignal) () <br> |
|  void | [**Finalize**](#function-finalize) () <br> |
|  void | [**Initialize**](#function-initialize) (bool isManualReset) <br> |
|  bool | [**IsManualReset**](#function-ismanualreset) () <br> |
|  bool | [**IsSignaled**](#function-issignaled) () <br> |
|   | [**LightEvent**](#function-lightevent-12) () <br> |
|   | [**LightEvent**](#function-lightevent-22) (bool isManualReset) <br> |
|  void | [**Pulse**](#function-pulse) () <br> |
|  void | [**Signal**](#function-signal) () <br> |
|  bool | [**TryWait**](#function-trywait) () <br> |
|  void | [**Wait**](#function-wait) () <br> |


















































## Protected Functions inherited from nn::util::ADLFireWall::NonCopyable

See [nn::util::ADLFireWall::NonCopyable](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md)

| Type | Name |
| ---: | :--- |
|   | [**NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable-12) () <br> |
|   | [**~NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable) () <br> |






## Public Functions Documentation




### function ClearSignal 

```C++
void nn::os::LightEvent::ClearSignal () 
```




<hr>



### function Finalize 

```C++
inline void nn::os::LightEvent::Finalize () 
```




<hr>



### function Initialize 

```C++
inline void nn::os::LightEvent::Initialize (
    bool isManualReset
) 
```




<hr>



### function IsManualReset 

```C++
inline bool nn::os::LightEvent::IsManualReset () 
```




<hr>



### function IsSignaled 

```C++
inline bool nn::os::LightEvent::IsSignaled () 
```




<hr>



### function LightEvent [1/2]

```C++
inline nn::os::LightEvent::LightEvent () 
```




<hr>



### function LightEvent [2/2]

```C++
inline nn::os::LightEvent::LightEvent (
    bool isManualReset
) 
```




<hr>



### function Pulse 

```C++
void nn::os::LightEvent::Pulse () 
```




<hr>



### function Signal 

```C++
void nn::os::LightEvent::Signal () 
```




<hr>



### function TryWait 

```C++
bool nn::os::LightEvent::TryWait () 
```




<hr>



### function Wait 

```C++
void nn::os::LightEvent::Wait () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/os/os_LightEvent.h`

