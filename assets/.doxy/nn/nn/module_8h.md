

# File module.h



[**FileList**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**module.h**](module_8h.md)

[Go to the source code of this file](module_8h_source.md)



* `#include <nn/util/detail/util_Symbol.h>`
































































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**NN\_MAKE\_MODULE**](module_8h.md#define-nn_make_module) (Variable, Company, Module) `const char Variable[] \_\_attribute\_\_((section(".module\_id"))) = "[SDK+" Company ":" Module "]"`<br> |
| define  | [**NN\_MAKE\_MODULE\_SDK**](module_8h.md#define-nn_make_module_sdk) (Variable, Module) `[**NN\_MAKE\_MODULE**](module_8h.md#define-nn_make_module)(Variable, "NINTENDO", Module)`<br> |
| define  | [**NN\_REFER\_MODULE**](module_8h.md#define-nn_refer_module) (Variable) `[**nnutilReferSymbol\_**](util___symbol_8h.md#function-nnutilrefersymbol_)(Variable)`<br> |

## Macro Definition Documentation





### define NN\_MAKE\_MODULE 

```C++
#define NN_MAKE_MODULE (
    Variable,
    Company,
    Module
) `const char Variable[] __attribute__((section(".module_id"))) = "[SDK+" Company ":" Module "]"`
```




<hr>



### define NN\_MAKE\_MODULE\_SDK 

```C++
#define NN_MAKE_MODULE_SDK (
    Variable,
    Module
) `NN_MAKE_MODULE (Variable, "NINTENDO", Module)`
```




<hr>



### define NN\_REFER\_MODULE 

```C++
#define NN_REFER_MODULE (
    Variable
) `nnutilReferSymbol_ (Variable)`
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/module.h`

