

# File crt0.cpp



[**FileList**](files.md) **>** [**crt0**](dir_2e40bb914eb64b354eaaaa48387a7993.md) **>** [**MPCore**](dir_165870d69a5bb9db0cc3d4369e8cb08b.md) **>** [**crt0.cpp**](crt0_8cpp.md)

[Go to the source code of this file](crt0_8cpp_source.md)



* `#include <nn/init/init_StartUp.h>`
* `#include <nn/module.h>`
* `#include <nn/svc/svc_Stub.h>`
* `#include <rt_locale.h>`
* `#include <rt_sys.h>`





















## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**u8**](types_8h.md#typedef-u8) | [**Image$$ZI$$ZI$$Base**](#variable-image$$zi$$zi$$base)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**Image$$ZI$$ZI$$Limit**](#variable-image$$zi$$zi$$limit)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  \_\_weak void | [**\_\_cpp\_initialize\_\_aeabi\_**](#function-__cpp_initialize__aeabi_) () <br> |
|  void \_\_asm | [**\_\_ctr\_start**](#function-__ctr_start) () <br> |
|  [**u32**](types_8h.md#typedef-u32) \* | [**\_\_rt\_locale**](#function-__rt_locale) (void) <br> |
|  void | [**nnMain**](#function-nnmain) () <br> |
|  void | [**nninitLocale**](#function-nninitlocale) () <br> |
|  void | [**nninitRegion**](#function-nninitregion) () <br> |
|  void | [**nninitStartUp**](#function-nninitstartup) () <br> |




























## Public Attributes Documentation




### variable Image$$ZI$$ZI$$Base 

```C++
u8 Image$$ZI$$ZI$$Base[];
```




<hr>



### variable Image$$ZI$$ZI$$Limit 

```C++
u8 Image$$ZI$$ZI$$Limit[];
```




<hr>
## Public Functions Documentation




### function \_\_cpp\_initialize\_\_aeabi\_ 

```C++
__weak void __cpp_initialize__aeabi_ () 
```




<hr>



### function \_\_ctr\_start 

```C++
void __asm __ctr_start () 
```




<hr>



### function \_\_rt\_locale 

```C++
u32 * __rt_locale (
    void
) 
```




<hr>



### function nnMain 

```C++
void nnMain () 
```




<hr>



### function nninitLocale 

```C++
void nninitLocale () 
```




<hr>



### function nninitRegion 

```C++
void nninitRegion () 
```




<hr>



### function nninitStartUp 

```C++
void nninitStartUp () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/sources/libraries/crt0/MPCore/crt0.cpp`

