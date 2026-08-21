

# File Result.h



[**FileList**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**Result.h**](_result_8h.md)

[Go to the source code of this file](_result_8h_source.md)
















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**nn**](namespacenn.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| struct | [**ConstRange**](structnn_1_1_const_range.md) &lt;TLevel, TSummary, TModule, TDescription, A, B&gt;<br> |
| struct | [**Const\_LM**](structnn_1_1_const___l_m.md) &lt;TLevel, TModule&gt;<br> |
| struct | [**Const**](structnn_1_1_const___l_m_1_1_const.md) &lt;TSummary, TDescription&gt;<br> |
| struct | [**Const\_LSM**](structnn_1_1_const___l_s_m.md) &lt;TLevel, TSummary, TModule&gt;<br> |
| struct | [**Const**](structnn_1_1_const___l_s_m_1_1_const.md) &lt;TDescription&gt;<br> |
| class | [**Result**](classnn_1_1_result.md) <br> |
| struct | [**Const**](structnn_1_1_result_1_1_const.md) &lt;TLevel, TSummary, TModule, TDescription&gt;<br> |
| struct | [**nnResult**](structnn_result.md) <br> |

















































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**NN\_RESULT\_DEF**](_result_8h.md#define-nn_result_def) (Type, Res, Sum, Desc) `/* multi line expression */`<br> |
| define  | [**NN\_RESULT\_DEF\_CONST**](_result_8h.md#define-nn_result_def_const) (result, level, summary, module, description) `typedef [**nn::Result::Const**](structnn_1_1_result_1_1_const.md)&lt;(level), (summary), (module), (description)&gt; result`<br> |
| define  | [**NN\_RESULT\_DEF\_CONST\_LM**](_result_8h.md#define-nn_result_def_const_lm) (result, sub, summary, description) `typedef sub::Const&lt;(summary), (description)&gt; result`<br> |
| define  | [**NN\_RESULT\_DEF\_CONST\_LSM**](_result_8h.md#define-nn_result_def_const_lsm) (result, sub, description) `typedef sub::Const&lt;(description)&gt; result`<br> |
| define  | [**NN\_RESULT\_DEF\_CONST\_RANGE**](_result_8h.md#define-nn_result_def_const_range) (result, level, summary, module, description, a, b) `typedef [**nn::Result::Const**](structnn_1_1_result_1_1_const.md)&lt;(level), (summary), (module), (description), (a), (b)&gt; result`<br> |
| define  | [**NN\_RESULT\_MAKE\_CONST\_LM**](_result_8h.md#define-nn_result_make_const_lm) (sub, level, module) `typedef [**::nn::Result::Const\_LM**](structnn_1_1_result_1_1_const___l_m.md)&lt;(level), (module)&gt; sub`<br> |
| define  | [**NN\_RESULT\_MAKE\_CONST\_LSM**](_result_8h.md#define-nn_result_make_const_lsm) (sub, level, summary, module) `typedef [**::nn::Result::Const\_LSM**](structnn_1_1_result_1_1_const___l_s_m.md)&lt;(level), (summary), (module)&gt; sub`<br> |
| define  | [**\_NN\_RESULT\_MAKE\_TYPE**](_result_8h.md#define-_nn_result_make_type) (name, e) `/* multi line expression */`<br> |

## Macro Definition Documentation





### define NN\_RESULT\_DEF 

```C++
#define NN_RESULT_DEF (
    Type,
    Res,
    Sum,
    Desc
) `/* multi line expression */`
```




<hr>



### define NN\_RESULT\_DEF\_CONST 

```C++
#define NN_RESULT_DEF_CONST (
    result,
    level,
    summary,
    module,
    description
) `typedef nn::Result::Const <(level), (summary), (module), (description)> result`
```




<hr>



### define NN\_RESULT\_DEF\_CONST\_LM 

```C++
#define NN_RESULT_DEF_CONST_LM (
    result,
    sub,
    summary,
    description
) `typedef sub::Const<(summary), (description)> result`
```




<hr>



### define NN\_RESULT\_DEF\_CONST\_LSM 

```C++
#define NN_RESULT_DEF_CONST_LSM (
    result,
    sub,
    description
) `typedef sub::Const<(description)> result`
```




<hr>



### define NN\_RESULT\_DEF\_CONST\_RANGE 

```C++
#define NN_RESULT_DEF_CONST_RANGE (
    result,
    level,
    summary,
    module,
    description,
    a,
    b
) `typedef nn::Result::Const <(level), (summary), (module), (description), (a), (b)> result`
```




<hr>



### define NN\_RESULT\_MAKE\_CONST\_LM 

```C++
#define NN_RESULT_MAKE_CONST_LM (
    sub,
    level,
    module
) `typedef ::nn::Result::Const_LM <(level), (module)> sub`
```




<hr>



### define NN\_RESULT\_MAKE\_CONST\_LSM 

```C++
#define NN_RESULT_MAKE_CONST_LSM (
    sub,
    level,
    summary,
    module
) `typedef ::nn::Result::Const_LSM <(level), (summary), (module)> sub`
```




<hr>



### define \_NN\_RESULT\_MAKE\_TYPE 

```C++
#define _NN_RESULT_MAKE_TYPE (
    name,
    e
) `/* multi line expression */`
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/Result.h`

