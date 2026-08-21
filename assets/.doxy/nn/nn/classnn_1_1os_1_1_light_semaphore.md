

# Class nn::os::LightSemaphore



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**os**](namespacenn_1_1os.md) **>** [**LightSemaphore**](classnn_1_1os_1_1_light_semaphore.md)





* `#include <os_LightSemaphore.h>`



Inherits the following classes: [nn::util::ADLFireWall::NonCopyable](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**Acquire**](#function-acquire) () <br> |
|  [**s32**](types_8h.md#typedef-s32) | [**GetCount**](#function-getcount) () const<br> |
|  [**s32**](types_8h.md#typedef-s32) | [**GetMax**](#function-getmax) () const<br> |
|  void | [**Initialize**](#function-initialize-12) ([**s32**](types_8h.md#typedef-s32) initialCount, [**s32**](types_8h.md#typedef-s32) maxCount) <br> |
|  void | [**Initialize**](#function-initialize-22) ([**s32**](types_8h.md#typedef-s32) initialCount) <br> |
|   | [**LightSemaphore**](#function-lightsemaphore) ([**s32**](types_8h.md#typedef-s32) initialCount, [**s32**](types_8h.md#typedef-s32) maxCount) <br> |
|  [**s32**](types_8h.md#typedef-s32) | [**Release**](#function-release) ([**s32**](types_8h.md#typedef-s32) releaseCount) <br> |
|  bool | [**TryAcquire**](#function-tryacquire) () <br> |
|   | [**~LightSemaphore**](#function-lightsemaphore) () <br> |


















































## Protected Functions inherited from nn::util::ADLFireWall::NonCopyable

See [nn::util::ADLFireWall::NonCopyable](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md)

| Type | Name |
| ---: | :--- |
|   | [**NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable-12) () <br> |
|   | [**~NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable) () <br> |






## Public Functions Documentation




### function Acquire 

```C++
inline void nn::os::LightSemaphore::Acquire () 
```




<hr>



### function GetCount 

```C++
inline s32 nn::os::LightSemaphore::GetCount () const
```




<hr>



### function GetMax 

```C++
inline s32 nn::os::LightSemaphore::GetMax () const
```




<hr>



### function Initialize [1/2]

```C++
inline void nn::os::LightSemaphore::Initialize (
    s32 initialCount,
    s32 maxCount
) 
```




<hr>



### function Initialize [2/2]

```C++
inline void nn::os::LightSemaphore::Initialize (
    s32 initialCount
) 
```




<hr>



### function LightSemaphore 

```C++
inline nn::os::LightSemaphore::LightSemaphore (
    s32 initialCount,
    s32 maxCount
) 
```




<hr>



### function Release 

```C++
s32 nn::os::LightSemaphore::Release (
    s32 releaseCount
) 
```




<hr>



### function TryAcquire 

```C++
inline bool nn::os::LightSemaphore::TryAcquire () 
```




<hr>



### function ~LightSemaphore 

```C++
inline nn::os::LightSemaphore::~LightSemaphore () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/os/os_LightSemaphore.h`

