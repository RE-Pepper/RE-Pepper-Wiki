

# Namespace nn::dbg



[**Namespace List**](namespaces.md) **>** [**nn**](namespacenn.md) **>** [**dbg**](namespacenn_1_1dbg.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**detail**](namespacenn_1_1dbg_1_1detail.md) <br> |




## Public Types

| Type | Name |
| ---: | :--- |
| typedef void(\* | [**BreakHandler**](#typedef-breakhandler)  <br> |
| enum  | [**BreakReason**](#enum-breakreason)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  [**Result**](classnn_1_1_result.md) | [**Break**](#function-break) ([**BreakReason**](namespacenn_1_1dbg.md#enum-breakreason) reason) <br> |
|  [**Result**](classnn_1_1_result.md) | [**Break**](#function-break) () <br> |
|  void | [**Panic**](#function-panic) () <br> |
|  void | [**PrintErrorMessageHeader**](#function-printerrormessageheader) ([**nndbgBreakReason**](dbg___enum_8h.md#enum-nndbgbreakreason) reason, const char \* filename, int lineno) <br> |




























## Public Types Documentation




### typedef BreakHandler 

```C++
typedef void(* nn::dbg::BreakHandler) (BreakReason reason, const Result *pResult, const char *filename, int lineno, const char *message, va_list vlist);
```




<hr>



### enum BreakReason 

```C++
enum nn::dbg::BreakReason {
    BREAK_REASON_PANIC = 0,
    BREAK_REASON_ASSERT = 1,
    BREAK_REASON_USER = 2,
    BREAK_REASON_LOAD_RO = 3,
    BREAK_REASON_UNLOAD_RO = 4,
    BREAK_REASON_MAX_BIT = 2147483648
};
```




<hr>
## Public Functions Documentation




### function Break 

```C++
Result nn::dbg::Break (
    BreakReason reason
) 
```




<hr>



### function Break 

```C++
inline Result nn::dbg::Break () 
```




<hr>



### function Panic 

```C++
void nn::dbg::Panic () 
```




<hr>



### function PrintErrorMessageHeader 

```C++
void nn::dbg::PrintErrorMessageHeader (
    nndbgBreakReason reason,
    const char * filename,
    int lineno
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/dbg/dbg_Break.h`

