

# File project\_globals.h



[**FileList**](files.md) **>** [**Game**](dir_c33286056d2acf479cd8641ef845fec1.md) **>** [**project\_globals.h**](project__globals_8h.md)

[Go to the source code of this file](project__globals_8h_source.md)



* `#include <nn/types.h>`
































































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**NN\_SWITCH\_DISABLE\_ASSERT\_WARNING\_FOR\_SDK**](project__globals_8h.md#define-nn_switch_disable_assert_warning_for_sdk)  `1`<br> |
| define  | [**NN\_SWITCH\_DISABLE\_DEBUG\_PRINTING\_FOR\_SDK**](project__globals_8h.md#define-nn_switch_disable_debug_printing_for_sdk)  `1`<br> |
| define  | [**RP\_SHUTUP**](project__globals_8h.md#define-rp_shutup)  `\_Pragma("diag\_suppress 177,550,940")`<br> |
| define  | [**S**](project__globals_8h.md#define-s) (x) `[**S\_**](project__globals_8h.md#define-s_)(x)`<br> |
| define  | [**S\_**](project__globals_8h.md#define-s_) (x) `#x`<br> |
| define  | [**\_SECT\_RO**](project__globals_8h.md#define-_sect_ro)  `".constdata." \_\_BASE\_FILE\_NAME\_\_`<br> |
| define  | [**\_SECT\_RW**](project__globals_8h.md#define-_sect_rw)  `".data." \_\_BASE\_FILE\_NAME\_\_`<br> |
| define  | [**\_SECT\_ZI**](project__globals_8h.md#define-_sect_zi)  `".bss." \_\_BASE\_FILE\_NAME\_\_`<br> |
| define  | [**\_\_clrex**](project__globals_8h.md#define-__clrex) () <br> |
| define  | [**\_\_weak**](project__globals_8h.md#define-__weak)  <br> |
| define  | [**asm**](project__globals_8h.md#define-asm) (Name) `Name`<br> |
| define  | [**asm\_ext**](project__globals_8h.md#define-asm_ext) (Name, Sect) `Name`<br> |
| define  | [**force\_func\_section**](project__globals_8h.md#define-force_func_section) (Symbol) <br> |
| define  | [**force\_section**](project__globals_8h.md#define-force_section) (Section) <br> |
| define  | [**var**](project__globals_8h.md#define-var) (Namespace, Name, Type) `Type Name`<br> |
| define  | [**varc**](project__globals_8h.md#define-varc) (Namespace, Class, Name, Type) `Type Class::Name`<br> |
| define  | [**varcg**](project__globals_8h.md#define-varcg) (Name, Class, Type) `Type Class::Name`<br> |
| define  | [**varg**](project__globals_8h.md#define-varg) (Name, Type) `Type Name`<br> |

## Macro Definition Documentation





### define NN\_SWITCH\_DISABLE\_ASSERT\_WARNING\_FOR\_SDK 

```C++
#define NN_SWITCH_DISABLE_ASSERT_WARNING_FOR_SDK `1`
```




<hr>



### define NN\_SWITCH\_DISABLE\_DEBUG\_PRINTING\_FOR\_SDK 

```C++
#define NN_SWITCH_DISABLE_DEBUG_PRINTING_FOR_SDK `1`
```




<hr>



### define RP\_SHUTUP 

```C++
#define RP_SHUTUP `_Pragma("diag_suppress 177,550,940")`
```




<hr>



### define S 

```C++
#define S (
    x
) `S_ (x)`
```




<hr>



### define S\_ 

```C++
#define S_ (
    x
) `#x`
```




<hr>



### define \_SECT\_RO 

```C++
#define _SECT_RO `".constdata." __BASE_FILE_NAME__`
```




<hr>



### define \_SECT\_RW 

```C++
#define _SECT_RW `".data." __BASE_FILE_NAME__`
```




<hr>



### define \_SECT\_ZI 

```C++
#define _SECT_ZI `".bss." __BASE_FILE_NAME__`
```




<hr>



### define \_\_clrex 

```C++
#define __clrex (
    
) 
```




<hr>



### define \_\_weak 

```C++
#define __weak 
```




<hr>



### define asm 

```C++
#define asm (
    Name
) `Name`
```




<hr>



### define asm\_ext 

```C++
#define asm_ext (
    Name,
    Sect
) `Name`
```




<hr>



### define force\_func\_section 

```C++
#define force_func_section (
    Symbol
) 
```




<hr>



### define force\_section 

```C++
#define force_section (
    Section
) 
```




<hr>



### define var 

```C++
#define var (
    Namespace,
    Name,
    Type
) `Type Name`
```




<hr>



### define varc 

```C++
#define varc (
    Namespace,
    Class,
    Name,
    Type
) `Type Class::Name`
```




<hr>



### define varcg 

```C++
#define varcg (
    Name,
    Class,
    Type
) `Type Class::Name`
```




<hr>



### define varg 

```C++
#define varg (
    Name,
    Type
) `Type Name`
```




<hr>

------------------------------
The documentation for this class was generated from the following file `Game/project_globals.h`

