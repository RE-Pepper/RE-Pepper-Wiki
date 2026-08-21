

# File dbg\_PrintResult.cpp



[**FileList**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**dbg**](dir_f5f58bbdde99f1620da85a5357502216.md) **>** [**dbg\_PrintResult.cpp**](dbg___print_result_8cpp.md)

[Go to the source code of this file](dbg___print_result_8cpp_source.md)



* `#include <nn/dbg/dbg_DebugString.h>`
* `#include <nn/dbg/dbg_PrintResult.h>`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**nn**](namespacenn.md) <br> |
| namespace | [**dbg**](namespacenn_1_1dbg.md) <br> |
| namespace | [**detail**](namespacenn_1_1dbg_1_1detail.md) <br> |



















































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**CALL\_GET\_RESULT\_DESCRIPTION**](dbg___print_result_8cpp.md#define-call_get_result_description) (module, e) `case Result::e: desc = ::nn::module::GetResultDescriptionStringImpl (result); break;`<br> |
| define  | [**ENTRY\_GET\_RESULT\_DESCRIPTION**](dbg___print_result_8cpp.md#define-entry_get_result_description) (Func, Desc) `/* multi line expression */`<br> |
| define  | [**ENTRY\_GET\_RESULT\_DESCRIPTION\_DESC**](dbg___print_result_8cpp.md#define-entry_get_result_description_desc) (Desc) `[**ENTRY\_GET\_RESULT\_DESCRIPTION**](dbg___print_result_8cpp.md#define-entry_get_result_description) (GetDescription, Desc)`<br> |
| define  | [**ENTRY\_GET\_RESULT\_DESCRIPTION\_FALLBACK**](dbg___print_result_8cpp.md#define-entry_get_result_description_fallback)  `return "&lt;unknown&gt;"`<br> |
| define  | [**ENTRY\_GET\_RESULT\_DESCRIPTION\_LVL**](dbg___print_result_8cpp.md#define-entry_get_result_description_lvl) (Desc) `[**ENTRY\_GET\_RESULT\_DESCRIPTION**](dbg___print_result_8cpp.md#define-entry_get_result_description) (GetSummary, Desc)`<br> |
| define  | [**ENTRY\_GET\_RESULT\_DESCRIPTION\_MOD**](dbg___print_result_8cpp.md#define-entry_get_result_description_mod) (Desc) `[**ENTRY\_GET\_RESULT\_DESCRIPTION**](dbg___print_result_8cpp.md#define-entry_get_result_description) (GetModule, Desc)`<br> |
| define  | [**ENTRY\_GET\_RESULT\_DESCRIPTION\_SUM**](dbg___print_result_8cpp.md#define-entry_get_result_description_sum) (Desc) `[**ENTRY\_GET\_RESULT\_DESCRIPTION**](dbg___print_result_8cpp.md#define-entry_get_result_description) (GetSummary, Desc)`<br> |
| define  | [**PREDEFINE\_GET\_RESULT\_DESCRIPTION**](dbg___print_result_8cpp.md#define-predefine_get_result_description) (module) `/* multi line expression */`<br> |

## Macro Definition Documentation





### define CALL\_GET\_RESULT\_DESCRIPTION 

```C++
#define CALL_GET_RESULT_DESCRIPTION (
    module,
    e
) `case Result::e: desc = ::nn::module::GetResultDescriptionStringImpl (result); break;`
```




<hr>



### define ENTRY\_GET\_RESULT\_DESCRIPTION 

```C++
#define ENTRY_GET_RESULT_DESCRIPTION (
    Func,
    Desc
) `/* multi line expression */`
```




<hr>



### define ENTRY\_GET\_RESULT\_DESCRIPTION\_DESC 

```C++
#define ENTRY_GET_RESULT_DESCRIPTION_DESC (
    Desc
) `ENTRY_GET_RESULT_DESCRIPTION (GetDescription, Desc)`
```




<hr>



### define ENTRY\_GET\_RESULT\_DESCRIPTION\_FALLBACK 

```C++
#define ENTRY_GET_RESULT_DESCRIPTION_FALLBACK `return "<unknown>"`
```




<hr>



### define ENTRY\_GET\_RESULT\_DESCRIPTION\_LVL 

```C++
#define ENTRY_GET_RESULT_DESCRIPTION_LVL (
    Desc
) `ENTRY_GET_RESULT_DESCRIPTION (GetSummary, Desc)`
```




<hr>



### define ENTRY\_GET\_RESULT\_DESCRIPTION\_MOD 

```C++
#define ENTRY_GET_RESULT_DESCRIPTION_MOD (
    Desc
) `ENTRY_GET_RESULT_DESCRIPTION (GetModule, Desc)`
```




<hr>



### define ENTRY\_GET\_RESULT\_DESCRIPTION\_SUM 

```C++
#define ENTRY_GET_RESULT_DESCRIPTION_SUM (
    Desc
) `ENTRY_GET_RESULT_DESCRIPTION (GetSummary, Desc)`
```




<hr>



### define PREDEFINE\_GET\_RESULT\_DESCRIPTION 

```C++
#define PREDEFINE_GET_RESULT_DESCRIPTION (
    module
) `/* multi line expression */`
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/sources/libraries/dbg/dbg_PrintResult.cpp`

