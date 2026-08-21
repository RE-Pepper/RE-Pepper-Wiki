

# Struct nn::os::ReadOnlySharedInfo



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**os**](namespacenn_1_1os.md) **>** [**ReadOnlySharedInfo**](structnn_1_1os_1_1_read_only_shared_info.md)





* `#include <os_SharedInfo.h>`

















## Public Types

| Type | Name |
| ---: | :--- |
| enum  | [**Flags**](#enum-flags)  <br> |




## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**bit8**](types_8h.md#typedef-bit8) | [**bootEnv**](#variable-bootenv)  <br> |
|  [**bit32**](types_8h.md#typedef-bit32) | [**coreVersion**](#variable-coreversion)  <br> |
|  [**bit8**](types_8h.md#typedef-bit8) | [**deviceEnv**](#variable-deviceenv)  <br> |
|  [**bit32**](types_8h.md#typedef-bit32) | [**firstCoreVersion**](#variable-firstcoreversion)  <br> |
|  [**ProgramID**](namespacenn.md#typedef-programid) | [**firstMainBootProgram**](#variable-firstmainbootprogram)  <br> |
|  [**bit32**](types_8h.md#typedef-bit32) | [**firstRevision**](#variable-firstrevision)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**firstVersionMajor**](#variable-firstversionmajor)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**firstVersionMicro**](#variable-firstversionmicro)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**firstVersionMinor**](#variable-firstversionminor)  <br> |
|  [**bit8**](types_8h.md#typedef-bit8) | [**firstVersionReserve**](#variable-firstversionreserve)  <br> |
|  [**FlagsEnum4**](structnn_1_1os_1_1_flags_enum4.md)&lt; [**Flags**](structnn_1_1os_1_1_read_only_shared_info.md#enum-flags) &gt; | [**flags**](#variable-flags)  <br> |
|  [**bit32**](types_8h.md#typedef-bit32) | [**kParamAck**](#variable-kparamack)  <br> |
|  [**bit32**](types_8h.md#typedef-bit32) | [**kParamCurrent**](#variable-kparamcurrent)  <br> |
|  [**bit32**](types_8h.md#typedef-bit32) | [**kParamValues**](#variable-kparamvalues)  <br> |
|  [**bit8**](types_8h.md#typedef-bit8) | [**previousMode**](#variable-previousmode)  <br> |
|  [**u32**](types_8h.md#typedef-u32) | [**revision**](#variable-revision)  <br> |
|  int | [**unk**](#variable-unk)  <br> |
|  int | [**unk1**](#variable-unk1)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**versionMajor**](#variable-versionmajor)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**versionMicro**](#variable-versionmicro)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**versionMinor**](#variable-versionminor)  <br> |
|  [**bit8**](types_8h.md#typedef-bit8) | [**versionReserve**](#variable-versionreserve)  <br> |












































## Public Types Documentation




### enum Flags 

```C++
enum nn::os::ReadOnlySharedInfo::Flags {
    FLAGS_SAVE_MODE = 1,
    FLAGS_MAX_BITS = 2147483648
};
```




<hr>
## Public Attributes Documentation




### variable bootEnv 

```C++
bit8 nn::os::ReadOnlySharedInfo::bootEnv;
```




<hr>



### variable coreVersion 

```C++
bit32 nn::os::ReadOnlySharedInfo::coreVersion;
```




<hr>



### variable deviceEnv 

```C++
bit8 nn::os::ReadOnlySharedInfo::deviceEnv;
```




<hr>



### variable firstCoreVersion 

```C++
bit32 nn::os::ReadOnlySharedInfo::firstCoreVersion;
```




<hr>



### variable firstMainBootProgram 

```C++
ProgramID nn::os::ReadOnlySharedInfo::firstMainBootProgram;
```




<hr>



### variable firstRevision 

```C++
bit32 nn::os::ReadOnlySharedInfo::firstRevision;
```




<hr>



### variable firstVersionMajor 

```C++
u8 nn::os::ReadOnlySharedInfo::firstVersionMajor;
```




<hr>



### variable firstVersionMicro 

```C++
u8 nn::os::ReadOnlySharedInfo::firstVersionMicro;
```




<hr>



### variable firstVersionMinor 

```C++
u8 nn::os::ReadOnlySharedInfo::firstVersionMinor;
```




<hr>



### variable firstVersionReserve 

```C++
bit8 nn::os::ReadOnlySharedInfo::firstVersionReserve;
```




<hr>



### variable flags 

```C++
FlagsEnum4<Flags> nn::os::ReadOnlySharedInfo::flags;
```




<hr>



### variable kParamAck 

```C++
bit32 nn::os::ReadOnlySharedInfo::kParamAck[4];
```




<hr>



### variable kParamCurrent 

```C++
bit32 nn::os::ReadOnlySharedInfo::kParamCurrent[4];
```




<hr>



### variable kParamValues 

```C++
bit32 nn::os::ReadOnlySharedInfo::kParamValues[8];
```




<hr>



### variable previousMode 

```C++
bit8 nn::os::ReadOnlySharedInfo::previousMode;
```




<hr>



### variable revision 

```C++
u32 nn::os::ReadOnlySharedInfo::revision;
```




<hr>



### variable unk 

```C++
int nn::os::ReadOnlySharedInfo::unk;
```




<hr>



### variable unk1 

```C++
int nn::os::ReadOnlySharedInfo::unk1;
```




<hr>



### variable versionMajor 

```C++
u8 nn::os::ReadOnlySharedInfo::versionMajor;
```




<hr>



### variable versionMicro 

```C++
u8 nn::os::ReadOnlySharedInfo::versionMicro;
```




<hr>



### variable versionMinor 

```C++
u8 nn::os::ReadOnlySharedInfo::versionMinor;
```




<hr>



### variable versionReserve 

```C++
bit8 nn::os::ReadOnlySharedInfo::versionReserve;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/os/os_SharedInfo.h`

