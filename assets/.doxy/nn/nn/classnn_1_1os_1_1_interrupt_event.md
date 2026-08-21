

# Class nn::os::InterruptEvent



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**os**](namespacenn_1_1os.md) **>** [**InterruptEvent**](classnn_1_1os_1_1_interrupt_event.md)





* `#include <os_Synchronization.h>`



Inherits the following classes: [nn::os::WaitObject](classnn_1_1os_1_1_wait_object.md)


Inherited by the following classes: [nn::os::EventBase](classnn_1_1os_1_1_event_base.md),  [nn::os::Semaphore](structnn_1_1os_1_1_semaphore.md)




























































































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**InterruptEvent**](#function-interruptevent) () <br> |
|   | [**~InterruptEvent**](#function-interruptevent) () <br> |


## Public Functions inherited from nn::os::WaitObject

See [nn::os::WaitObject](classnn_1_1os_1_1_wait_object.md)

| Type | Name |
| ---: | :--- |
|   | [**WaitObject**](classnn_1_1os_1_1_wait_object.md#function-waitobject) () <br> |
|  void | [**WaitOne**](classnn_1_1os_1_1_wait_object.md#function-waitone-12) () <br> |
|  bool | [**WaitOne**](classnn_1_1os_1_1_wait_object.md#function-waitone-22) ([**fnd::TimeSpan**](classnn_1_1fnd_1_1_time_span.md) timeout) <br> |
|  [**Result**](classnn_1_1_result.md) | [**WaitOneImpl**](classnn_1_1os_1_1_wait_object.md#function-waitoneimpl) ([**s64**](types_8h.md#typedef-s64) nanoSecondsTimeout) <br> |
|   | [**~WaitObject**](classnn_1_1os_1_1_wait_object.md#function-waitobject) () <br> |


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






## Public Static Functions inherited from nn::os::WaitObject

See [nn::os::WaitObject](classnn_1_1os_1_1_wait_object.md)

| Type | Name |
| ---: | :--- |
|  [**s32**](types_8h.md#typedef-s32) | [**WaitAny**](classnn_1_1os_1_1_wait_object.md#function-waitany) ([**WaitObject**](classnn_1_1os_1_1_wait_object.md) \*\* objs, [**s32**](types_8h.md#typedef-s32) numObjects) <br> |


























































































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




### function InterruptEvent 

```C++
inline nn::os::InterruptEvent::InterruptEvent () 
```




<hr>



### function ~InterruptEvent 

```C++
inline nn::os::InterruptEvent::~InterruptEvent () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/os/os_Synchronization.h`

