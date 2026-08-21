

# Class nn::srv::detail::HandlerManager



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**srv**](namespacenn_1_1srv.md) **>** [**detail**](namespacenn_1_1srv_1_1detail.md) **>** [**HandlerManager**](classnn_1_1srv_1_1detail_1_1_handler_manager.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**NotificationHandler**](classnn_1_1srv_1_1_notification_handler.md) \* | [**Find**](#function-find) ([**bit32**](types_8h.md#typedef-bit32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**Register**](#function-register) ([**NotificationHandler**](classnn_1_1srv_1_1_notification_handler.md) \* pHandler, [**bit32**](types_8h.md#typedef-bit32)) <br> |
|  [**NotificationHandler**](classnn_1_1srv_1_1_notification_handler.md) \* | [**Unregister**](#function-unregister) ([**bit32**](types_8h.md#typedef-bit32)) <br> |




























## Public Functions Documentation




### function Find 

```C++
inline NotificationHandler * nn::srv::detail::HandlerManager::Find (
    bit32
) 
```




<hr>



### function Register 

```C++
inline Result nn::srv::detail::HandlerManager::Register (
    NotificationHandler * pHandler,
    bit32
) 
```




<hr>



### function Unregister 

```C++
inline NotificationHandler * nn::srv::detail::HandlerManager::Unregister (
    bit32
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/sources/libraries/srv/srv_Api.cpp`

