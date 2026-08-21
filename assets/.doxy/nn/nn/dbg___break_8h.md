

# File dbg\_Break.h



[**FileList**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**dbg**](dir_8674e25a187048eae8b9b07d931da2b2.md) **>** [**dbg\_Break.h**](dbg___break_8h.md)

[Go to the source code of this file](dbg___break_8h_source.md)



* `#include <nn/Result.h>`
* `#include <nn/dbg/dbg_Enum.h>`













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
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/dbg/dbg_Break.h`

