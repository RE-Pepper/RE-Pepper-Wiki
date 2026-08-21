

# Class nn::hid::CTR::HidBase



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**hid**](namespacenn_1_1hid.md) **>** [**CTR**](namespacenn_1_1hid_1_1_c_t_r.md) **>** [**HidBase**](classnn_1_1hid_1_1_c_t_r_1_1_hid_base.md)





* `#include <hid_HidBase.h>`



Inherits the following classes: [nn::os::EventBase](classnn_1_1os_1_1_event_base.md)






































































































































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**uptr**](types_8h.md#typedef-uptr) | [**GetResource**](#function-getresource) () const<br> |
|   | [**HidBase**](#function-hidbase) () <br> |
|  void | [**SetResource**](#function-setresource) ([**uptr**](types_8h.md#typedef-uptr) resource) <br> |
|   | [**~HidBase**](#function-hidbase) () <br> |


## Public Functions inherited from nn::os::EventBase

See [nn::os::EventBase](classnn_1_1os_1_1_event_base.md)

| Type | Name |
| ---: | :--- |
|  void | [**ClearSignal**](classnn_1_1os_1_1_event_base.md#function-clearsignal) () <br> |
|   | [**EventBase**](classnn_1_1os_1_1_event_base.md#function-eventbase-12) () <br> |
|   | [**EventBase**](classnn_1_1os_1_1_event_base.md#function-eventbase-22) ([**ResetType**](namespacenn_1_1os.md#enum-resettype) resetType) <br> |
|  void | [**Initialize**](classnn_1_1os_1_1_event_base.md#function-initialize) ([**ResetType**](namespacenn_1_1os.md#enum-resettype) resetType) <br> |
|  void | [**Signal**](classnn_1_1os_1_1_event_base.md#function-signal) () <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryInitialize**](classnn_1_1os_1_1_event_base.md#function-tryinitialize) ([**ResetType**](namespacenn_1_1os.md#enum-resettype) resetType) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryInitializeImpl**](classnn_1_1os_1_1_event_base.md#function-tryinitializeimpl) ([**ResetType**](namespacenn_1_1os.md#enum-resettype) resetType) <br> |
|   | [**~EventBase**](classnn_1_1os_1_1_event_base.md#function-eventbase) () <br> |


## Public Functions inherited from nn::os::InterruptEvent

See [nn::os::InterruptEvent](classnn_1_1os_1_1_interrupt_event.md)

| Type | Name |
| ---: | :--- |
|   | [**InterruptEvent**](classnn_1_1os_1_1_interrupt_event.md#function-interruptevent) () <br> |
|   | [**~InterruptEvent**](classnn_1_1os_1_1_interrupt_event.md#function-interruptevent) () <br> |


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




### function GetResource 

```C++
inline uptr nn::hid::CTR::HidBase::GetResource () const
```




<hr>



### function HidBase 

```C++
inline nn::hid::CTR::HidBase::HidBase () 
```




<hr>



### function SetResource 

```C++
inline void nn::hid::CTR::HidBase::SetResource (
    uptr resource
) 
```




<hr>



### function ~HidBase 

```C++
inline nn::hid::CTR::HidBase::~HidBase () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/hid/CTR/hid_HidBase.h`

