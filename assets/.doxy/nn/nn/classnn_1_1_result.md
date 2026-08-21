

# Class nn::Result



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**Result**](classnn_1_1_result.md)





* `#include <Result.h>`





Inherited by the following classes: [nn::ConstRange](structnn_1_1_const_range.md),  [nn::Result::Const](structnn_1_1_result_1_1_const.md)










## Classes

| Type | Name |
| ---: | :--- |
| struct | [**Const**](structnn_1_1_result_1_1_const.md) &lt;TLevel, TSummary, TModule, TDescription&gt;<br> |
| struct | [**ConstRange**](structnn_1_1_result_1_1_const_range.md) &lt;[**Level**](classnn_1_1_result.md#enum-level), [**Summary**](classnn_1_1_result.md#enum-summary), [**Module**](classnn_1_1_result.md#enum-module), int, int, int&gt;<br> |
| struct | [**Const\_LM**](structnn_1_1_result_1_1_const___l_m.md) &lt;[**Level**](classnn_1_1_result.md#enum-level), [**Module**](classnn_1_1_result.md#enum-module)&gt;<br> |
| struct | [**Const\_LSM**](structnn_1_1_result_1_1_const___l_s_m.md) &lt;[**Level**](classnn_1_1_result.md#enum-level), [**Summary**](classnn_1_1_result.md#enum-summary), [**Module**](classnn_1_1_result.md#enum-module)&gt;<br> |


## Public Types

| Type | Name |
| ---: | :--- |
| enum  | [**Description**](#enum-description)  <br> |
| enum  | [**Level**](#enum-level)  <br> |
| enum  | [**Module**](#enum-module)  <br> |
| enum  | [**Summary**](#enum-summary)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  [**bit32**](types_8h.md#typedef-bit32) | [**GetCodeBits**](#function-getcodebits) ([**bit32**](types_8h.md#typedef-bit32) mask, [**s32**](types_8h.md#typedef-s32) shift) const<br> |
|  int | [**GetDescription**](#function-getdescription) () const<br> |
|  [**Level**](classnn_1_1_result.md#enum-level) | [**GetLevel**](#function-getlevel) () const<br> |
|  [**Module**](classnn_1_1_result.md#enum-module) | [**GetModule**](#function-getmodule) () const<br> |
|  [**bit32**](types_8h.md#typedef-bit32) | [**GetPrintableBits**](#function-getprintablebits) () const<br> |
|  [**Summary**](classnn_1_1_result.md#enum-summary) | [**GetSummary**](#function-getsummary) () const<br> |
|  bool | [**IsFailure**](#function-isfailure) () const<br> |
|  bool | [**IsSuccess**](#function-issuccess) () const<br> |
|   | [**Result**](#function-result-14) ([**bit32**](types_8h.md#typedef-bit32) code) <br> |
|   | [**Result**](#function-result-24) () <br> |
|   | [**Result**](#function-result-34) ([**Level**](classnn_1_1_result.md#enum-level) level, [**Summary**](classnn_1_1_result.md#enum-summary) summary, [**Module**](classnn_1_1_result.md#enum-module) module, int description) <br> |
|   | [**Result**](#function-result-44) ([**nnResult**](structnn_result.md) result) <br> |
|   | [**operator nnResult**](#function-operator-nnresult) () <br> |
|  bool | [**operator!=**](#function-operator) (const [**Result**](classnn_1_1_result.md) & rhs) <br> |
|  bool | [**operator==**](#function-operator_1) (const [**Result**](classnn_1_1_result.md) & rhs) <br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**bit32**](types_8h.md#typedef-bit32) | [**m\_Code**](#variable-m_code)  <br> |




















## Public Types Documentation




### enum Description 

```C++
enum nn::Result::Description {
    DESCRIPTION_SUCCESS = 0,
    DESCRIPTION_INVALID_SELECTION = 1000,
    DESCRIPTION_TOO_LARGE = 1001,
    DESCRIPTION_NOT_AUTHORIZED = 1002,
    DESCRIPTION_ALREADY_DONE = 1003,
    DESCRIPTION_INVALID_SIZE = 1004,
    DESCRIPTION_INVALID_ENUM_VALUE = 1005,
    DESCRIPTION_INVALID_COMBINATION = 1006,
    DESCRIPTION_NO_DATA = 1007,
    DESCRIPTION_BUSY = 1008,
    DESCRIPTION_MISALIGNED_ADDRESS = 1009,
    DESCRIPTION_MISALIGNED_SIZE = 1010,
    DESCRIPTION_OUT_OF_MEMORY = 1011,
    DESCRIPTION_NOT_IMPLEMENTED = 1012,
    DESCRIPTION_INVALID_ADDRESS = 1013,
    DESCRIPTION_INVALID_POINTER = 1014,
    DESCRIPTION_INVALID_HANDLE = 1015,
    DESCRIPTION_NOT_INITIALIZED = 1016,
    DESCRIPTION_ALREADY_INITIALIZED = 1017,
    DESCRIPTION_NOT_FOUND = 1018,
    DESCRIPTION_CANCEL_REQUESTED = 1019,
    DESCRIPTION_ALREADY_EXISTS = 1020,
    DESCRIPTION_OUT_OF_RANGE = 1021,
    DESCRIPTION_TIMEOUT = 1022,
    DESCRIPTION_INVALID_RESULT_VALUE = 1023
};
```




<hr>



### enum Level 

```C++
enum nn::Result::Level {
    LEVEL_INFO = 1,
    LEVEL_SUCCESS = 0,
    LEVEL_FATAL = -1,
    LEVEL_RESET = -2,
    LEVEL_REINIT = -3,
    LEVEL_USAGE = -4,
    LEVEL_PERMANENT = -5,
    LEVEL_TEMPORARY = -6,
    LEVEL_STATUS = -7,
    LEVEL_END
};
```




<hr>



### enum Module 

```C++
enum nn::Result::Module {
    MODULE_COMMON,
    MODULE_NN_KERNEL,
    MODULE_NN_UTIL,
    MODULE_NN_FILE_SERVER,
    MODULE_NN_LOADER_SERVER,
    MODULE_NN_TCB,
    MODULE_NN_OS,
    MODULE_NN_DBG,
    MODULE_NN_DMNT,
    MODULE_NN_PDN,
    MODULE_NN_GX,
    MODULE_NN_I2C,
    MODULE_NN_GPIO,
    MODULE_NN_DD,
    MODULE_NN_CODEC,
    MODULE_NN_SPI,
    MODULE_NN_PXI,
    MODULE_NN_FS,
    MODULE_NN_DI,
    MODULE_NN_HID,
    MODULE_NN_CAMERA,
    MODULE_NN_PI,
    MODULE_NN_PM,
    MODULE_NN_PMLOW,
    MODULE_NN_FSI,
    MODULE_NN_SRV,
    MODULE_NN_NDM,
    MODULE_NN_NWM,
    MODULE_NN_SOCKET,
    MODULE_NN_LDR,
    MODULE_NN_ACC,
    MODULE_NN_ROMFS,
    MODULE_NN_AM,
    MODULE_NN_HIO,
    MODULE_NN_UPDATER,
    MODULE_NN_MIC,
    MODULE_NN_FND,
    MODULE_NN_MP,
    MODULE_NN_MPWL,
    MODULE_NN_AC,
    MODULE_NN_HTTP,
    MODULE_NN_DSP,
    MODULE_NN_SND,
    MODULE_NN_DLP,
    MODULE_NN_HIOLOW,
    MODULE_NN_CSND,
    MODULE_NN_SSL,
    MODULE_NN_AMLOW,
    MODULE_NN_NEX,
    MODULE_NN_FRIENDS,
    MODULE_NN_RDT,
    MODULE_NN_APPLET,
    MODULE_NN_NIM,
    MODULE_NN_PTM,
    MODULE_NN_MIDI,
    MODULE_NN_MC,
    MODULE_NN_SWC,
    MODULE_NN_FATFS,
    MODULE_NN_NGC,
    MODULE_NN_CARD,
    MODULE_NN_CARDNOR,
    MODULE_NN_SDMC,
    MODULE_NN_BOSS,
    MODULE_NN_DBM,
    MODULE_NN_CFG,
    MODULE_NN_PS,
    MODULE_NN_CEC,
    MODULE_NN_IR,
    MODULE_NN_UDS,
    MODULE_NN_PL,
    MODULE_NN_CUP,
    MODULE_NN_GYROSCOPE,
    MODULE_NN_MCU,
    MODULE_NN_NS,
    MODULE_NN_NEWS,
    MODULE_NN_RO,
    MODULE_NN_GD,
    MODULE_NN_CARDSPI,
    MODULE_NN_EC,
    MODULE_NN_WEBBRS,
    MODULE_NN_TEST,
    MODULE_NN_ENC,
    MODULE_NN_PIA,
    MODULE_APPLICATION = 254,
    MODULE_INVALID_RESULT_VALUE
};
```




<hr>



### enum Summary 

```C++
enum nn::Result::Summary {
    SUMMARY_SUCCESS = 0,
    SUMMARY_NOTHING_HAPPENED = 1,
    SUMMARY_WOULD_BLOCK = 2,
    SUMMARY_OUT_OF_RESOURCE = 3,
    SUMMARY_NOT_FOUND = 4,
    SUMMARY_INVALID_STATE = 5,
    SUMMARY_NOT_SUPPORTED = 6,
    SUMMARY_INVALID_ARGUMENT = 7,
    SUMMARY_WRONG_ARGUMENT = 8,
    SUMMARY_CANCELLED = 9,
    SUMMARY_STATUS_CHANGED = 10,
    SUMMARY_INTERNAL = 11,
    SUMMARY_INVALID_RESULT_VALUE = 63
};
```




<hr>
## Public Functions Documentation




### function GetCodeBits 

```C++
inline bit32 nn::Result::GetCodeBits (
    bit32 mask,
    s32 shift
) const
```




<hr>



### function GetDescription 

```C++
inline int nn::Result::GetDescription () const
```




<hr>



### function GetLevel 

```C++
inline Level nn::Result::GetLevel () const
```




<hr>



### function GetModule 

```C++
inline Module nn::Result::GetModule () const
```




<hr>



### function GetPrintableBits 

```C++
inline bit32 nn::Result::GetPrintableBits () const
```




<hr>



### function GetSummary 

```C++
inline Summary nn::Result::GetSummary () const
```




<hr>



### function IsFailure 

```C++
inline bool nn::Result::IsFailure () const
```




<hr>



### function IsSuccess 

```C++
inline bool nn::Result::IsSuccess () const
```




<hr>



### function Result [1/4]

```C++
inline nn::Result::Result (
    bit32 code
) 
```




<hr>



### function Result [2/4]

```C++
inline nn::Result::Result () 
```




<hr>



### function Result [3/4]

```C++
inline nn::Result::Result (
    Level level,
    Summary summary,
    Module module,
    int description
) 
```




<hr>



### function Result [4/4]

```C++
inline nn::Result::Result (
    nnResult result
) 
```




<hr>



### function operator nnResult 

```C++
inline nn::Result::operator nnResult () 
```




<hr>



### function operator!= 

```C++
inline bool nn::Result::operator!= (
    const Result & rhs
) 
```




<hr>



### function operator== 

```C++
inline bool nn::Result::operator== (
    const Result & rhs
) 
```




<hr>
## Protected Attributes Documentation




### variable m\_Code 

```C++
bit32 nn::Result::m_Code;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/Result.h`

