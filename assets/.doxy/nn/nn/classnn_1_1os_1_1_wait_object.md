

# Class nn::os::WaitObject



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**os**](namespacenn_1_1os.md) **>** [**WaitObject**](classnn_1_1os_1_1_wait_object.md)





* `#include <os_Synchronization.h>`



Inherits the following classes: [nn::os::HandleObject](classnn_1_1os_1_1_handle_object.md)


Inherited by the following classes: [nn::os::InterruptEvent](classnn_1_1os_1_1_interrupt_event.md),  [nn::os::Thread](classnn_1_1os_1_1_thread.md)








































































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**WaitObject**](#function-waitobject) () <br> |
|  void | [**WaitOne**](#function-waitone-12) () <br> |
|  bool | [**WaitOne**](#function-waitone-22) ([**fnd::TimeSpan**](classnn_1_1fnd_1_1_time_span.md) timeout) <br> |
|  [**Result**](classnn_1_1_result.md) | [**WaitOneImpl**](#function-waitoneimpl) ([**s64**](types_8h.md#typedef-s64) nanoSecondsTimeout) <br> |
|   | [**~WaitObject**](#function-waitobject) () <br> |


## Public Functions inherited from nn::os::HandleObject

See [nn::os::HandleObject](classnn_1_1os_1_1_handle_object.md)

| Type | Name |
| ---: | :--- |
|  void | [**ClearHandle**](classnn_1_1os_1_1_handle_object.md#function-clearhandle) () <br> |
|  void | [**Close**](classnn_1_1os_1_1_handle_object.md#function-close) () <br> |
|  void | [**Finalize**](classnn_1_1os_1_1_handle_object.md#function-finalize) () <br> |
|   | [**HandleObject**](classnn_1_1os_1_1_handle_object.md#function-handleobject) () <br> |
|  void | [**SetHandle**](classnn_1_1os_1_1_handle_object.md#function-sethandle) ([**Handle**](classnn_1_1_handle.md) handle) <br> |
|   | [**~HandleObject**](classnn_1_1os_1_1_handle_object.md#function-handleobject) () <br> |




## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**s32**](types_8h.md#typedef-s32) | [**WaitAny**](#function-waitany) ([**WaitObject**](classnn_1_1os_1_1_wait_object.md) \*\* objs, [**s32**](types_8h.md#typedef-s32) numObjects) <br> |




































































## Protected Functions inherited from nn::os::HandleObject

See [nn::os::HandleObject](classnn_1_1os_1_1_handle_object.md)

| Type | Name |
| ---: | :--- |
|  [**Handle**](classnn_1_1_handle.md) | [**GetHandle**](classnn_1_1os_1_1_handle_object.md#function-gethandle) () const<br> |
|  bool | [**IsValid**](classnn_1_1os_1_1_handle_object.md#function-isvalid) () const<br> |


## Protected Functions inherited from nn::util::ADLFireWall::NonCopyable

See [nn::util::ADLFireWall::NonCopyable](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md)

| Type | Name |
| ---: | :--- |
|   | [**NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable-12) () <br> |
|   | [**~NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable) () <br> |








## Public Functions Documentation




### function WaitObject 

```C++
inline nn::os::WaitObject::WaitObject () 
```




<hr>



### function WaitOne [1/2]

```C++
inline void nn::os::WaitObject::WaitOne () 
```




<hr>



### function WaitOne [2/2]

```C++
inline bool nn::os::WaitObject::WaitOne (
    fnd::TimeSpan timeout
) 
```




<hr>



### function WaitOneImpl 

```C++
inline Result nn::os::WaitObject::WaitOneImpl (
    s64 nanoSecondsTimeout
) 
```




<hr>



### function ~WaitObject 

```C++
inline nn::os::WaitObject::~WaitObject () 
```




<hr>
## Public Static Functions Documentation




### function WaitAny 

```C++
static inline s32 nn::os::WaitObject::WaitAny (
    WaitObject ** objs,
    s32 numObjects
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/os/os_Synchronization.h`

