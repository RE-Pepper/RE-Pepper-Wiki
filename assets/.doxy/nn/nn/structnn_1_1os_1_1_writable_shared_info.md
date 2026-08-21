

# Struct nn::os::WritableSharedInfo



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**os**](namespacenn_1_1os.md) **>** [**WritableSharedInfo**](structnn_1_1os_1_1_writable_shared_info.md)





* `#include <os_SharedInfo.h>`





















## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**u8**](types_8h.md#typedef-u8) | [**batteryState**](#variable-batterystate)  <br> |
|  [**ProgramID**](namespacenn.md#typedef-programid) | [**currentSystemMenu**](#variable-currentsystemmenu)  <br> |
|  bool | [**displayModeLockFlag**](#variable-displaymodelockflag)  <br> |
|  [**ProgramID**](namespacenn.md#typedef-programid) | [**firstSystemMenu**](#variable-firstsystemmenu)  <br> |
|  bool | [**isHeadphoneInserted**](#variable-isheadphoneinserted)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**mcuInfoRegisters\_10**](#variable-mcuinforegisters_10)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**mcuTargetInfo**](#variable-mcutargetinfo)  <br> |
|  [**bit8**](types_8h.md#typedef-bit8) | [**reserved\_0x006**](#variable-reserved_0x006)  <br> |
|  [**bit8**](types_8h.md#typedef-bit8) | [**reserved\_0x070**](#variable-reserved_0x070)  <br> |
|  [**bit8**](types_8h.md#typedef-bit8) | [**reserved\_0x087**](#variable-reserved_0x087)  <br> |
|  [**bit8**](types_8h.md#typedef-bit8) | [**reserved\_0x0b0**](#variable-reserved_0x0b0)  <br> |
|  [**bit8**](types_8h.md#typedef-bit8) | [**reserved\_0x0c1**](#variable-reserved_0x0c1)  <br> |
|  [**RtcSwcInfo**](structnn_1_1os_1_1_rtc_swc_info.md) | [**rtcSwcInfo**](#variable-rtcswcinfo)  <br> |
|  [**s32**](types_8h.md#typedef-s32) | [**rtcValidNumber**](#variable-rtcvalidnumber)  <br> |
|  [**f32**](types_8h.md#typedef-f32) | [**svr2Volume**](#variable-svr2volume)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**targetHardware**](#variable-targethardware)  <br> |
|  [**bit8**](types_8h.md#typedef-bit8) | [**wirelessInfo**](#variable-wirelessinfo)  <br> |












































## Public Attributes Documentation




### variable batteryState 

```C++
u8 nn::os::WritableSharedInfo::batteryState;
```




<hr>



### variable currentSystemMenu 

```C++
ProgramID nn::os::WritableSharedInfo::currentSystemMenu;
```




<hr>



### variable displayModeLockFlag 

```C++
bool nn::os::WritableSharedInfo::displayModeLockFlag;
```




<hr>



### variable firstSystemMenu 

```C++
ProgramID nn::os::WritableSharedInfo::firstSystemMenu;
```




<hr>



### variable isHeadphoneInserted 

```C++
bool nn::os::WritableSharedInfo::isHeadphoneInserted;
```




<hr>



### variable mcuInfoRegisters\_10 

```C++
u8 nn::os::WritableSharedInfo::mcuInfoRegisters_10;
```




<hr>



### variable mcuTargetInfo 

```C++
u8 nn::os::WritableSharedInfo::mcuTargetInfo;
```




<hr>



### variable reserved\_0x006 

```C++
bit8 nn::os::WritableSharedInfo::reserved_0x006[25];
```




<hr>



### variable reserved\_0x070 

```C++
bit8 nn::os::WritableSharedInfo::reserved_0x070[16];
```




<hr>



### variable reserved\_0x087 

```C++
bit8 nn::os::WritableSharedInfo::reserved_0x087[26];
```




<hr>



### variable reserved\_0x0b0 

```C++
bit8 nn::os::WritableSharedInfo::reserved_0x0b0[16];
```




<hr>



### variable reserved\_0x0c1 

```C++
bit8 nn::os::WritableSharedInfo::reserved_0x0c1[31];
```




<hr>



### variable rtcSwcInfo 

```C++
RtcSwcInfo nn::os::WritableSharedInfo::rtcSwcInfo[2];
```




<hr>



### variable rtcValidNumber 

```C++
s32 nn::os::WritableSharedInfo::rtcValidNumber;
```




<hr>



### variable svr2Volume 

```C++
f32 nn::os::WritableSharedInfo::svr2Volume;
```




<hr>



### variable targetHardware 

```C++
u8 nn::os::WritableSharedInfo::targetHardware;
```




<hr>



### variable wirelessInfo 

```C++
bit8 nn::os::WritableSharedInfo::wirelessInfo[16];
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/os/os_SharedInfo.h`

