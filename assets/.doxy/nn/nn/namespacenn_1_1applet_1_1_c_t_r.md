

# Namespace nn::applet::CTR



[**Namespace List**](namespaces.md) **>** [**nn**](namespacenn.md) **>** [**applet**](namespacenn_1_1applet.md) **>** [**CTR**](namespacenn_1_1applet_1_1_c_t_r.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| enum  | [**AppJumpType**](#enum-appjumptype)  <br> |
| typedef [**AppJumpType**](namespacenn_1_1applet_1_1_c_t_r.md#enum-appjumptype) | [**AppletAppJumpType**](#typedef-appletappjumptype)  <br> |
| typedef [**bit32**](types_8h.md#typedef-bit32) | [**AppletAttr**](#typedef-appletattr)  <br> |
| typedef void(\* | [**AppletAwakeCallback**](#typedef-appletawakecallback)  <br> |
| typedef void(\* | [**AppletCloseAppletCallback**](#typedef-appletcloseappletcallback)  <br> |
| typedef void(\* | [**AppletCloseCallback**](#typedef-appletclosecallback)  <br> |
| typedef [**DataManagementScene**](namespacenn_1_1applet_1_1_c_t_r.md#enum-datamanagementscene) | [**AppletDataManagementScene**](#typedef-appletdatamanagementscene)  <br> |
| typedef [**DisplayBufferMode**](namespacenn_1_1applet_1_1_c_t_r.md#enum-displaybuffermode) | [**AppletDisplayBufferMode**](#typedef-appletdisplaybuffermode)  <br> |
| typedef void(\* | [**AppletDspSleepCallback**](#typedef-appletdspsleepcallback)  <br> |
| typedef void(\* | [**AppletDspWakeUpCallback**](#typedef-appletdspwakeupcallback)  <br> |
| typedef bool(\* | [**AppletHomeButtonCallback**](#typedef-applethomebuttoncallback)  <br> |
| typedef [**bit32**](types_8h.md#typedef-bit32) | [**AppletId**](#typedef-appletid)  <br> |
| typedef void(\* | [**AppletMessageCallback**](#typedef-appletmessagecallback)  <br> |
| typedef [**MsetScene**](namespacenn_1_1applet_1_1_c_t_r.md#enum-msetscene) | [**AppletMsetScene**](#typedef-appletmsetscene)  <br> |
| typedef [**OrderToCloseState**](namespacenn_1_1applet_1_1_c_t_r.md#enum-ordertoclosestate) | [**AppletOrderToCloseState**](#typedef-appletordertoclosestate)  <br> |
| typedef [**ParentalControlsScene**](namespacenn_1_1applet_1_1_c_t_r.md#enum-parentalcontrolsscene) | [**AppletParentalControlsScene**](#typedef-appletparentalcontrolsscene)  <br> |
| enum  | [**AppletPos**](#enum-appletpos)  <br> |
| typedef void(\* | [**AppletPowerButtonCallback**](#typedef-appletpowerbuttoncallback)  <br> |
| typedef [**PowerButtonState**](namespacenn_1_1applet_1_1_c_t_r.md#enum-powerbuttonstate) | [**AppletPowerButtonState**](#typedef-appletpowerbuttonstate)  <br> |
| typedef [**QueryReply**](namespacenn_1_1applet_1_1_c_t_r.md#enum-queryreply) | [**AppletQueryReply**](#typedef-appletqueryreply)  <br> |
| typedef void(\* | [**AppletReleaseMemoryCallback**](#typedef-appletreleasememorycallback)  <br> |
| typedef void(\* | [**AppletRequestMemoryCallback**](#typedef-appletrequestmemorycallback)  <br> |
| typedef void(\* | [**AppletShutdownCallback**](#typedef-appletshutdowncallback)  <br> |
| typedef [**ShutdownState**](namespacenn_1_1applet_1_1_c_t_r.md#enum-shutdownstate) | [**AppletShutdownState**](#typedef-appletshutdownstate)  <br> |
| typedef void(\* | [**AppletSleepCanceledCallback**](#typedef-appletsleepcanceledcallback)  <br> |
| typedef [**AppletQueryReply**](namespacenn_1_1applet_1_1_c_t_r.md#enum-queryreply)(\* | [**AppletSleepQueryCallback**](#typedef-appletsleepquerycallback)  <br> |
| typedef void(\* | [**AppletTransitionCallback**](#typedef-applettransitioncallback)  <br> |
| typedef [**WakeupState**](namespacenn_1_1applet_1_1_c_t_r.md#enum-wakeupstate) | [**AppletWakeupState**](#typedef-appletwakeupstate)  <br> |
| enum  | [**DataManagementScene**](#enum-datamanagementscene)  <br> |
| enum  | [**DisplayBufferMode**](#enum-displaybuffermode)  <br> |
| enum  | [**HomeButtonState**](#enum-homebuttonstate)  <br> |
| enum  | [**MsetScene**](#enum-msetscene)  <br> |
| enum  | [**OrderToCloseState**](#enum-ordertoclosestate)  <br> |
| enum  | [**ParentalControlsScene**](#enum-parentalcontrolsscene)  <br> |
| enum  | [**PowerButtonState**](#enum-powerbuttonstate)  <br> |
| enum  | [**QueryReply**](#enum-queryreply)  <br> |
| enum  | [**ShutdownState**](#enum-shutdownstate)  <br> |
| enum  | [**SleepNotificationState**](#enum-sleepnotificationstate)  <br> |
| enum  | [**WakeupState**](#enum-wakeupstate)  <br> |




## Public Attributes

| Type | Name |
| ---: | :--- |
|  const [**Handle**](classnn_1_1_handle.md) | [**HANDLE\_NONE**](#variable-handle_none)  <br> |
|  const [**fnd::TimeSpan**](classnn_1_1fnd_1_1_time_span.md) | [**NO\_WAIT**](#variable-no_wait)  <br> |
|  const [**fnd::TimeSpan**](classnn_1_1fnd_1_1_time_span.md) | [**WAIT\_INFINITE**](#variable-wait_infinite)  <br> |












































## Public Types Documentation




### enum AppJumpType 

```C++
enum nn::applet::CTR::AppJumpType {
    JUMP_OTHER = 0,
    JUMP_CALLER = 1,
    JUMP_SELF = 2
};
```




<hr>



### typedef AppletAppJumpType 

```C++
typedef AppJumpType nn::applet::CTR::AppletAppJumpType;
```




<hr>



### typedef AppletAttr 

```C++
typedef bit32 nn::applet::CTR::AppletAttr;
```




<hr>



### typedef AppletAwakeCallback 

```C++
typedef void(* nn::applet::CTR::AppletAwakeCallback) ();
```




<hr>



### typedef AppletCloseAppletCallback 

```C++
typedef void(* nn::applet::CTR::AppletCloseAppletCallback) (uptr);
```




<hr>



### typedef AppletCloseCallback 

```C++
typedef void(* nn::applet::CTR::AppletCloseCallback) (Handle);
```




<hr>



### typedef AppletDataManagementScene 

```C++
typedef DataManagementScene nn::applet::CTR::AppletDataManagementScene;
```




<hr>



### typedef AppletDisplayBufferMode 

```C++
typedef DisplayBufferMode nn::applet::CTR::AppletDisplayBufferMode;
```




<hr>



### typedef AppletDspSleepCallback 

```C++
typedef void(* nn::applet::CTR::AppletDspSleepCallback) (uptr);
```




<hr>



### typedef AppletDspWakeUpCallback 

```C++
typedef void(* nn::applet::CTR::AppletDspWakeUpCallback) (AppletQueryReply);
```




<hr>



### typedef AppletHomeButtonCallback 

```C++
typedef bool(* nn::applet::CTR::AppletHomeButtonCallback) (uptr, AppletId, u8 *, size_t);
```




<hr>



### typedef AppletId 

```C++
typedef bit32 nn::applet::CTR::AppletId;
```




<hr>



### typedef AppletMessageCallback 

```C++
typedef void(* nn::applet::CTR::AppletMessageCallback) (uptr, size_t);
```




<hr>



### typedef AppletMsetScene 

```C++
typedef MsetScene nn::applet::CTR::AppletMsetScene;
```




<hr>



### typedef AppletOrderToCloseState 

```C++
typedef OrderToCloseState nn::applet::CTR::AppletOrderToCloseState;
```




<hr>



### typedef AppletParentalControlsScene 

```C++
typedef ParentalControlsScene nn::applet::CTR::AppletParentalControlsScene;
```




<hr>



### enum AppletPos 

```C++
enum nn::applet::CTR::AppletPos {
    POS_APP = 0,
    POS_APPLIB = 1,
    POS_SYS = 2,
    POS_SYSLIB = 3,
    POS_RESIDENT = 4,
    POS_MAX = 5,
    POS_NONE = -1
};
```




<hr>



### typedef AppletPowerButtonCallback 

```C++
typedef void(* nn::applet::CTR::AppletPowerButtonCallback) (uptr);
```




<hr>



### typedef AppletPowerButtonState 

```C++
typedef PowerButtonState nn::applet::CTR::AppletPowerButtonState;
```




<hr>



### typedef AppletQueryReply 

```C++
typedef QueryReply nn::applet::CTR::AppletQueryReply;
```




<hr>



### typedef AppletReleaseMemoryCallback 

```C++
typedef void(* nn::applet::CTR::AppletReleaseMemoryCallback) (uptr);
```




<hr>



### typedef AppletRequestMemoryCallback 

```C++
typedef void(* nn::applet::CTR::AppletRequestMemoryCallback) (uptr);
```




<hr>



### typedef AppletShutdownCallback 

```C++
typedef void(* nn::applet::CTR::AppletShutdownCallback) (uptr);
```




<hr>



### typedef AppletShutdownState 

```C++
typedef ShutdownState nn::applet::CTR::AppletShutdownState;
```




<hr>



### typedef AppletSleepCanceledCallback 

```C++
typedef void(* nn::applet::CTR::AppletSleepCanceledCallback) (uptr);
```




<hr>



### typedef AppletSleepQueryCallback 

```C++
typedef AppletQueryReply(* nn::applet::CTR::AppletSleepQueryCallback) (uptr);
```




<hr>



### typedef AppletTransitionCallback 

```C++
typedef void(* nn::applet::CTR::AppletTransitionCallback) (uptr);
```




<hr>



### typedef AppletWakeupState 

```C++
typedef WakeupState nn::applet::CTR::AppletWakeupState;
```




<hr>



### enum DataManagementScene 

```C++
enum nn::applet::CTR::DataManagementScene {
    DATA_MANAGEMENT_TOP = 0,
    DATA_MANAGEMENT_STREETPASS = 1
};
```




<hr>



### enum DisplayBufferMode 

```C++
enum nn::applet::CTR::DisplayBufferMode {
    FORMAT_R8G8B8A8 = 0,
    FORMAT_R8G8B8 = 1,
    FORMAT_R5G6B5 = 2,
    FORMAT_R5G5B5A1 = 3,
    FORAMT_R4G4B4A4 = 4,
    FORMAT_UNIMPORTABLE = 4294967295
};
```




<hr>



### enum HomeButtonState 

```C++
enum nn::applet::CTR::HomeButtonState {
    HOME_BUTTON_NONE = 0,
    HOME_BUTTON_SINGLE_PRESSED = 1,
    HOME_BUTTON_DOUBLE_PRESSED = 2
};
```




<hr>



### enum MsetScene 

```C++
enum nn::applet::CTR::MsetScene {
    MSET_INTERNET_SETTING_TOP = 110,
    MSET_PARENTAL_CONTROLS_TOP = 111,
    MSET_PARENTAL_CONTROLS_COPPACS = 112,
    MSET_DATA_MANAGEMENT_TOP = 113,
    MSET_DATA_MANAGEMENT_STREETPASS = 117,
    MSET_SCENE_INVALID_VALUE = 4294967295
};
```




<hr>



### enum OrderToCloseState 

```C++
enum nn::applet::CTR::OrderToCloseState {
    ORDER_TO_CLOSE_STATE_NONE = 0,
    ORDER_TO_CLOSE_STATE_RECEIVED = 1
};
```




<hr>



### enum ParentalControlsScene 

```C++
enum nn::applet::CTR::ParentalControlsScene {
    PARENTAL_CONTROLS_TOP = 0,
    PARENTAL_CONTROLS_COPPACS = 1
};
```




<hr>



### enum PowerButtonState 

```C++
enum nn::applet::CTR::PowerButtonState {
    POWER_BUTTON_STATE_NONE = 0,
    POWER_BUTTON_STATE_CLICK = 1
};
```




<hr>



### enum QueryReply 

```C++
enum nn::applet::CTR::QueryReply {
    REPLY_REJECT = 0,
    REPLY_ACCEPT = 1,
    REPLY_LATER = 2
};
```




<hr>



### enum ShutdownState 

```C++
enum nn::applet::CTR::ShutdownState {
    SHUTDOWN_STATE_NONE = 0,
    SHUTDOWN_STATE_RECEIVED = 1
};
```




<hr>



### enum SleepNotificationState 

```C++
enum nn::applet::CTR::SleepNotificationState {
    NOTIFY_NONE = 0,
    NOTIFY_SLEEP_QUERY = 1,
    NOTIFY_SLEEP_ACCEPT = 2,
    NOTIFY_SLEEP_REJECT = 3,
    NOTIFY_SLEEP_ACCEPTED = 4,
    NOTIFY_AWAKE = 5
};
```




<hr>



### enum WakeupState 

```C++
enum nn::applet::CTR::WakeupState {
    WAKEUP_SKIP = 0,
    WAKEUP_TO_START = 1,
    WAKEUP_BY_EXIT = 2,
    WAKEUP_BY_PAUSE = 3,
    WAKEUP_BY_CANCEL = 4,
    WAKEUP_BY_CANCELALL = 5,
    WAKEUP_BY_POWER_BUTTON_CLICK = 6,
    WAKEUP_TO_JUMP_HOME = 7,
    WAKEUP_TO_JUMP_APPLICATION = 8,
    WAKEUP_TO_LAUNCH_APPLICATION = 9,
    WAKEUP_BY_SUSPEND = 10,
    WAKEUP_STATE_MAX = 63,
    WAKEUP_BY_TIMEOUT = -1
};
```




<hr>
## Public Attributes Documentation




### variable HANDLE\_NONE 

```C++
const Handle nn::applet::CTR::HANDLE_NONE;
```




<hr>



### variable NO\_WAIT 

```C++
const fnd::TimeSpan nn::applet::CTR::NO_WAIT;
```




<hr>



### variable WAIT\_INFINITE 

```C++
const fnd::TimeSpan nn::applet::CTR::WAIT_INFINITE;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/applet/CTR/applet_Parameters.h`

