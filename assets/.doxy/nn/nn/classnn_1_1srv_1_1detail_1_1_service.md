

# Class nn::srv::detail::Service



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**srv**](namespacenn_1_1srv.md) **>** [**detail**](namespacenn_1_1srv_1_1detail.md) **>** [**Service**](classnn_1_1srv_1_1detail_1_1_service.md)





* `#include <srv_Service.h>`







































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**Result**](classnn_1_1_result.md) | [**EnableNotification**](#function-enablenotification) () <br> |
|  [**Result**](classnn_1_1_result.md) | [**GetNamedObject**](#function-getnamedobject) ([**Handle**](classnn_1_1_handle.md) \*, const [**char8**](types_8h.md#typedef-char8) \*, [**s32**](types_8h.md#typedef-s32), bool) <br> |
|  [**Result**](classnn_1_1_result.md) | [**GetServiceHandle**](#function-getservicehandle) ([**Handle**](classnn_1_1_handle.md) \*, const [**char8**](types_8h.md#typedef-char8) \*, [**s32**](types_8h.md#typedef-s32), [**bit32**](types_8h.md#typedef-bit32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**IsServiceRegistered**](#function-isserviceregistered) (bool \*, const [**char8**](types_8h.md#typedef-char8) \*, [**s32**](types_8h.md#typedef-s32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**PublishToSubscriber**](#function-publishtosubscriber) ([**bit32**](types_8h.md#typedef-bit32), [**bit32**](types_8h.md#typedef-bit32), [**bit32**](types_8h.md#typedef-bit32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**RegisterClient**](#function-registerclient) () <br> |
|  [**Result**](classnn_1_1_result.md) | [**RegisterObject**](#function-registerobject) ([**Handle**](classnn_1_1_handle.md), const [**char8**](types_8h.md#typedef-char8) \*, [**s32**](types_8h.md#typedef-s32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**RegisterService**](#function-registerservice) ([**Handle**](classnn_1_1_handle.md) \*, const [**char8**](types_8h.md#typedef-char8) \*, [**s32**](types_8h.md#typedef-s32), [**s32**](types_8h.md#typedef-s32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**Subscribe**](#function-subscribe) ([**bit32**](types_8h.md#typedef-bit32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**UnregisterObject**](#function-unregisterobject) (const [**char8**](types_8h.md#typedef-char8) \*, [**s32**](types_8h.md#typedef-s32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**UnregisterService**](#function-unregisterservice) (const [**char8**](types_8h.md#typedef-char8) \*, [**s32**](types_8h.md#typedef-s32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**Unsubscribe**](#function-unsubscribe) ([**bit32**](types_8h.md#typedef-bit32)) <br> |


























## Public Static Functions Documentation




### function EnableNotification 

```C++
static Result nn::srv::detail::Service::EnableNotification () 
```




<hr>



### function GetNamedObject 

```C++
static Result nn::srv::detail::Service::GetNamedObject (
    Handle *,
    const char8 *,
    s32,
    bool
) 
```




<hr>



### function GetServiceHandle 

```C++
static Result nn::srv::detail::Service::GetServiceHandle (
    Handle *,
    const char8 *,
    s32,
    bit32
) 
```




<hr>



### function IsServiceRegistered 

```C++
static Result nn::srv::detail::Service::IsServiceRegistered (
    bool *,
    const char8 *,
    s32
) 
```




<hr>



### function PublishToSubscriber 

```C++
static Result nn::srv::detail::Service::PublishToSubscriber (
    bit32,
    bit32,
    bit32
) 
```




<hr>



### function RegisterClient 

```C++
static Result nn::srv::detail::Service::RegisterClient () 
```




<hr>



### function RegisterObject 

```C++
static Result nn::srv::detail::Service::RegisterObject (
    Handle,
    const char8 *,
    s32
) 
```




<hr>



### function RegisterService 

```C++
static Result nn::srv::detail::Service::RegisterService (
    Handle *,
    const char8 *,
    s32,
    s32
) 
```




<hr>



### function Subscribe 

```C++
static Result nn::srv::detail::Service::Subscribe (
    bit32
) 
```




<hr>



### function UnregisterObject 

```C++
static Result nn::srv::detail::Service::UnregisterObject (
    const char8 *,
    s32
) 
```




<hr>



### function UnregisterService 

```C++
static Result nn::srv::detail::Service::UnregisterService (
    const char8 *,
    s32
) 
```




<hr>



### function Unsubscribe 

```C++
static Result nn::srv::detail::Service::Unsubscribe (
    bit32
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/srv/srv_Service.h`

