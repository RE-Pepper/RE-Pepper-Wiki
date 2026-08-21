

# Namespace nn::srv



[**Namespace List**](namespaces.md) **>** [**nn**](namespacenn.md) **>** [**srv**](namespacenn_1_1srv.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**detail**](namespacenn_1_1srv_1_1detail.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**EventNotificationHandlerBase**](classnn_1_1srv_1_1_event_notification_handler_base.md) &lt;class T&gt;<br> |
| class | [**NotificationHandler**](classnn_1_1srv_1_1_notification_handler.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| enum  | [**Description**](#enum-description)  <br> |
| typedef [**EventNotificationHandlerBase**](classnn_1_1srv_1_1_event_notification_handler_base.md)&lt; [**NotificationHandler**](classnn_1_1srv_1_1_notification_handler.md) \* &gt; | [**LightEventNotificationHandler**](#typedef-lighteventnotificationhandler)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  [**Result**](classnn_1_1_result.md) | [**GetServiceHandle**](#function-getservicehandle) ([**Handle**](classnn_1_1_handle.md) \* pOut, const [**char8**](types_8h.md#typedef-char8) \* pName, [**s32**](types_8h.md#typedef-s32) length, [**bit32**](types_8h.md#typedef-bit32) flags) <br> |
|  [**Result**](classnn_1_1_result.md) | [**GetServiceHandle**](#function-getservicehandle) ([**Handle**](classnn_1_1_handle.md) \* pOut, const [**char8**](types_8h.md#typedef-char8) \* pName) <br> |
|  [**Result**](classnn_1_1_result.md) | [**Initialize**](#function-initialize) () <br> |
|  [**Result**](classnn_1_1_result.md) | [**MakeInfoResult**](#function-makeinforesult) ([**Result::Summary**](classnn_1_1_result.md#enum-summary) summary, int description) <br> |
|  [**Result**](classnn_1_1_result.md) | [**MakePermanentResult**](#function-makepermanentresult) ([**Result::Summary**](classnn_1_1_result.md#enum-summary) summary, int description) <br> |
|  [**Result**](classnn_1_1_result.md) | [**ReceiveNotification**](#function-receivenotification) ([**bit32**](types_8h.md#typedef-bit32) pOut) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryGetServiceHandle**](#function-trygetservicehandle) ([**Handle**](classnn_1_1_handle.md) \* pOut, const [**char8**](types_8h.md#typedef-char8) \* pName) <br> |
|   | [**\_NN\_SRV\_MAKE\_RESULT**](#function-_nn_srv_make_result) (ResultAlreadyInitialized, SUMMARY\_INVALID\_STATE, Result::DESCRIPTION\_ALREADY\_INITIALIZED) <br> |
|   | [**\_NN\_SRV\_MAKE\_RESULT**](#function-_nn_srv_make_result) (ResultTooLongServiceName, SUMMARY\_WRONG\_ARGUMENT, DESCRIPTION\_TOO\_LONG\_SERVICE\_NAME) <br> |
|   | [**\_NN\_SRV\_MAKE\_RESULT**](#function-_nn_srv_make_result) (ResultNotInitialized, SUMMARY\_INVALID\_STATE, Result::DESCRIPTION\_NOT\_INITIALIZED) <br> |




























## Public Types Documentation




### enum Description 

```C++
enum nn::srv::Description {
    DESCRIPTION_FAILED_SYNCHRONIZATION = 1,
    DESCRIPTION_NO_SUCH_HANDLE = 2,
    DESCRIPTION_ALREADY_EXISTS = 3,
    DESCRIPTION_NOT_EXISTS = 4,
    DESCRIPTION_TOO_LONG_SERVICE_NAME = 5,
    DESCRIPTION_NOT_PERMITTED = 6,
    DESCRIPTION_INVALID_NAME = 7,
    DESCRIPTION_BUFFER_OVERFLOW = 8,
    DESCRIPTION_END
};
```




<hr>



### typedef LightEventNotificationHandler 

```C++
typedef EventNotificationHandlerBase<NotificationHandler*> nn::srv::LightEventNotificationHandler;
```




<hr>
## Public Functions Documentation




### function GetServiceHandle 

```C++
Result nn::srv::GetServiceHandle (
    Handle * pOut,
    const char8 * pName,
    s32 length,
    bit32 flags
) 
```




<hr>



### function GetServiceHandle 

```C++
inline Result nn::srv::GetServiceHandle (
    Handle * pOut,
    const char8 * pName
) 
```




<hr>



### function Initialize 

```C++
Result nn::srv::Initialize () 
```




<hr>



### function MakeInfoResult 

```C++
inline Result nn::srv::MakeInfoResult (
    Result::Summary summary,
    int description
) 
```




<hr>



### function MakePermanentResult 

```C++
inline Result nn::srv::MakePermanentResult (
    Result::Summary summary,
    int description
) 
```




<hr>



### function ReceiveNotification 

```C++
inline Result nn::srv::ReceiveNotification (
    bit32 pOut
) 
```




<hr>



### function TryGetServiceHandle 

```C++
inline Result nn::srv::TryGetServiceHandle (
    Handle * pOut,
    const char8 * pName
) 
```




<hr>



### function \_NN\_SRV\_MAKE\_RESULT 

```C++
nn::srv::_NN_SRV_MAKE_RESULT (
    ResultAlreadyInitialized,
    SUMMARY_INVALID_STATE,
    Result::DESCRIPTION_ALREADY_INITIALIZED
) 
```




<hr>



### function \_NN\_SRV\_MAKE\_RESULT 

```C++
nn::srv::_NN_SRV_MAKE_RESULT (
    ResultTooLongServiceName,
    SUMMARY_WRONG_ARGUMENT,
    DESCRIPTION_TOO_LONG_SERVICE_NAME
) 
```




<hr>



### function \_NN\_SRV\_MAKE\_RESULT 

```C++
nn::srv::_NN_SRV_MAKE_RESULT (
    ResultNotInitialized,
    SUMMARY_INVALID_STATE,
    Result::DESCRIPTION_NOT_INITIALIZED
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/srv/srv_Api.h`

