

# File assert.h



[**FileList**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**assert.h**](assert_8h.md)

[Go to the source code of this file](assert_8h_source.md)



* `#include <nn/Handle.h>`
* `#include <nn/dbg/dbg_Break.h>`
* `#include <nn/dbg/dbg_DebugString.h>`
































































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**NN\_ASSERT\_SDK**](assert_8h.md#define-nn_assert_sdk) (cond) `/* multi line expression */`<br> |
| define  | [**NN\_ASSERT\_SDK\_MAX**](assert_8h.md#define-nn_assert_sdk_max) (var, max) `/* multi line expression */`<br> |
| define  | [**NN\_ASSERT\_SDK\_MIN**](assert_8h.md#define-nn_assert_sdk_min) (var, min) `/* multi line expression */`<br> |
| define  | [**NN\_ASSERT\_SDK\_MSG**](assert_8h.md#define-nn_assert_sdk_msg) (cond, ...) `/* multi line expression */`<br> |
| define  | [**NN\_ASSERT\_SDK\_RESULT**](assert_8h.md#define-nn_assert_sdk_result) (cond, result) `/* multi line expression */`<br> |
| define  | [**NN\_PANIC\_SDK**](assert_8h.md#define-nn_panic_sdk) (...) `/* multi line expression */`<br> |

## Macro Definition Documentation





### define NN\_ASSERT\_SDK 

```C++
#define NN_ASSERT_SDK (
    cond
) `/* multi line expression */`
```




<hr>



### define NN\_ASSERT\_SDK\_MAX 

```C++
#define NN_ASSERT_SDK_MAX (
    var,
    max
) `/* multi line expression */`
```




<hr>



### define NN\_ASSERT\_SDK\_MIN 

```C++
#define NN_ASSERT_SDK_MIN (
    var,
    min
) `/* multi line expression */`
```




<hr>



### define NN\_ASSERT\_SDK\_MSG 

```C++
#define NN_ASSERT_SDK_MSG (
    cond,
    ...
) `/* multi line expression */`
```




<hr>



### define NN\_ASSERT\_SDK\_RESULT 

```C++
#define NN_ASSERT_SDK_RESULT (
    cond,
    result
) `/* multi line expression */`
```




<hr>



### define NN\_PANIC\_SDK 

```C++
#define NN_PANIC_SDK (
    ...
) `nn::dbg::detail::Printf ("Panic: %s:%d\n", __BASE_FILE__, __LINE__); \ nn::dbg::detail::Printf (__VA_ARGS__);                               \ nn::dbg::detail::Printf ("\n");                                      \ nn::dbg::Panic ();`
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/assert.h`

