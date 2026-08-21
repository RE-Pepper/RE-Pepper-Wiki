

# File dbg\_DebugString.cpp



[**FileList**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**dbg**](dir_f5f58bbdde99f1620da85a5357502216.md) **>** [**dbg\_DebugString.cpp**](dbg___debug_string_8cpp.md)

[Go to the source code of this file](dbg___debug_string_8cpp_source.md)



* `#include <cstdio>`
* `#include <nn/module.h>`
* `#include <nn/nstd/nstd_Printf.h>`
* `#include <nn/svc/svc_StubDbg.h>`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**nn**](namespacenn.md) <br> |
| namespace | [**dbg**](namespacenn_1_1dbg.md) <br> |
| namespace | [**detail**](namespacenn_1_1dbg_1_1detail.md) <br> |
























## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**nndbgDetailPrintf**](#function-nndbgdetailprintf) (const char \* fmt, ...) <br> |
|  void | [**nndbgDetailPutString**](#function-nndbgdetailputstring) (const char \* text, int length) <br> |
|  void | [**nndbgDetailTPrintf**](#function-nndbgdetailtprintf) (const char \* fmt, ...) <br> |
|  void | [**nndbgDetailTVPrintf**](#function-nndbgdetailtvprintf) (const char \* fmt, va\_list arg) <br> |
|  void | [**nndbgDetailVPrintf**](#function-nndbgdetailvprintf) (const char \* fmt, va\_list arg) <br> |
|  void | [**nndbgPrintWarning\_**](#function-nndbgprintwarning_) (const char \* filename, int lineno, const char \* fmt, ...) <br> |
|  void | [**nndbgTPrintWarning\_**](#function-nndbgtprintwarning_) (const char \* filename, int lineno, const char \* fmt, ...) <br> |




























## Public Functions Documentation




### function nndbgDetailPrintf 

```C++
void nndbgDetailPrintf (
    const char * fmt,
    ...
) 
```




<hr>



### function nndbgDetailPutString 

```C++
void nndbgDetailPutString (
    const char * text,
    int length
) 
```




<hr>



### function nndbgDetailTPrintf 

```C++
void nndbgDetailTPrintf (
    const char * fmt,
    ...
) 
```




<hr>



### function nndbgDetailTVPrintf 

```C++
void nndbgDetailTVPrintf (
    const char * fmt,
    va_list arg
) 
```




<hr>



### function nndbgDetailVPrintf 

```C++
void nndbgDetailVPrintf (
    const char * fmt,
    va_list arg
) 
```




<hr>



### function nndbgPrintWarning\_ 

```C++
void nndbgPrintWarning_ (
    const char * filename,
    int lineno,
    const char * fmt,
    ...
) 
```




<hr>



### function nndbgTPrintWarning\_ 

```C++
void nndbgTPrintWarning_ (
    const char * filename,
    int lineno,
    const char * fmt,
    ...
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/sources/libraries/dbg/dbg_DebugString.cpp`

