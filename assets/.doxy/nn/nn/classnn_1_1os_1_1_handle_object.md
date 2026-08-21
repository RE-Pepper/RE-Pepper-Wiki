

# Class nn::os::HandleObject



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**os**](namespacenn_1_1os.md) **>** [**HandleObject**](classnn_1_1os_1_1_handle_object.md)





* `#include <os_HandleObject.h>`



Inherits the following classes: [nn::util::ADLFireWall::NonCopyable](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md)


Inherited by the following classes: [nn::os::WaitObject](classnn_1_1os_1_1_wait_object.md)




















































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**ClearHandle**](#function-clearhandle) () <br> |
|  void | [**Close**](#function-close) () <br> |
|  void | [**Finalize**](#function-finalize) () <br> |
|   | [**HandleObject**](#function-handleobject) () <br> |
|  void | [**SetHandle**](#function-sethandle) ([**Handle**](classnn_1_1_handle.md) handle) <br> |
|   | [**~HandleObject**](#function-handleobject) () <br> |
















































## Protected Functions

| Type | Name |
| ---: | :--- |
|  [**Handle**](classnn_1_1_handle.md) | [**GetHandle**](#function-gethandle) () const<br> |
|  bool | [**IsValid**](#function-isvalid) () const<br> |


## Protected Functions inherited from nn::util::ADLFireWall::NonCopyable

See [nn::util::ADLFireWall::NonCopyable](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md)

| Type | Name |
| ---: | :--- |
|   | [**NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable-12) () <br> |
|   | [**~NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable) () <br> |






## Public Functions Documentation




### function ClearHandle 

```C++
inline void nn::os::HandleObject::ClearHandle () 
```




<hr>



### function Close 

```C++
inline void nn::os::HandleObject::Close () 
```




<hr>



### function Finalize 

```C++
inline void nn::os::HandleObject::Finalize () 
```




<hr>



### function HandleObject 

```C++
inline nn::os::HandleObject::HandleObject () 
```




<hr>



### function SetHandle 

```C++
inline void nn::os::HandleObject::SetHandle (
    Handle handle
) 
```




<hr>



### function ~HandleObject 

```C++
inline nn::os::HandleObject::~HandleObject () 
```




<hr>
## Protected Functions Documentation




### function GetHandle 

```C++
inline Handle nn::os::HandleObject::GetHandle () const
```




<hr>



### function IsValid 

```C++
inline bool nn::os::HandleObject::IsValid () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/os/os_HandleObject.h`

