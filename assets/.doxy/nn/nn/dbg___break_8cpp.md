

# File dbg\_Break.cpp



[**FileList**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**dbg**](dir_f5f58bbdde99f1620da85a5357502216.md) **>** [**dbg\_Break.cpp**](dbg___break_8cpp.md)

[Go to the source code of this file](dbg___break_8cpp_source.md)



* `#include <cstdarg>`
* `#include <nn/dbg/dbg_Break.h>`
* `#include <nn/dbg/dbg_DebugString.h>`
* `#include <nn/dbg/dbg_PrintResult.h>`
* `#include <nn/svc/svc_StubDbg.h>`
* `#include "nn/dbg/dbg_Enum.h"`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**nn**](namespacenn.md) <br> |
| namespace | [**dbg**](namespacenn_1_1dbg.md) <br> |
























## Public Functions

| Type | Name |
| ---: | :--- |
|  [**nnResult**](structnn_result.md) | [**nndbgBreak**](#function-nndbgbreak) ([**nndbgBreakReason**](dbg___enum_8h.md#enum-nndbgbreakreason) reason) <br> |
|  void | [**nndbgBreakWithMessage\_**](#function-nndbgbreakwithmessage_) ([**nndbgBreakReason**](dbg___enum_8h.md#enum-nndbgbreakreason) reason, const char \* filename, int lineno, const char \* fmt, ...) <br> |
|  void | [**nndbgBreakWithResultMessage\_**](#function-nndbgbreakwithresultmessage_) ([**nndbgBreakReason**](dbg___enum_8h.md#enum-nndbgbreakreason) reason, [**nnResult**](structnn_result.md) result, const char \* filename, int lineno, const char \* fmt, ...) <br> |
|  void | [**nndbgBreakWithResultTMessage\_**](#function-nndbgbreakwithresulttmessage_) ([**nndbgBreakReason**](dbg___enum_8h.md#enum-nndbgbreakreason) reason, [**nnResult**](structnn_result.md) result, const char \* filename, int lineno, const char \* fmt, ...) <br> |
|  void | [**nndbgBreakWithTMessage\_**](#function-nndbgbreakwithtmessage_) ([**nndbgBreakReason**](dbg___enum_8h.md#enum-nndbgbreakreason) reason, const char \* filename, int lineno, const char \* fmt, ...) <br> |
|  void | [**nndbgPanic**](#function-nndbgpanic) () <br> |




























## Public Functions Documentation




### function nndbgBreak 

```C++
nnResult nndbgBreak (
    nndbgBreakReason reason
) 
```




<hr>



### function nndbgBreakWithMessage\_ 

```C++
void nndbgBreakWithMessage_ (
    nndbgBreakReason reason,
    const char * filename,
    int lineno,
    const char * fmt,
    ...
) 
```




<hr>



### function nndbgBreakWithResultMessage\_ 

```C++
void nndbgBreakWithResultMessage_ (
    nndbgBreakReason reason,
    nnResult result,
    const char * filename,
    int lineno,
    const char * fmt,
    ...
) 
```




<hr>



### function nndbgBreakWithResultTMessage\_ 

```C++
void nndbgBreakWithResultTMessage_ (
    nndbgBreakReason reason,
    nnResult result,
    const char * filename,
    int lineno,
    const char * fmt,
    ...
) 
```




<hr>



### function nndbgBreakWithTMessage\_ 

```C++
void nndbgBreakWithTMessage_ (
    nndbgBreakReason reason,
    const char * filename,
    int lineno,
    const char * fmt,
    ...
) 
```




<hr>



### function nndbgPanic 

```C++
void nndbgPanic () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/sources/libraries/dbg/dbg_Break.cpp`

