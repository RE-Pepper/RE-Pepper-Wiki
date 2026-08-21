

# Namespace nn



[**Namespace List**](namespaces.md) **>** [**nn**](namespacenn.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**applet**](namespacenn_1_1applet.md) <br> |
| namespace | [**cfg**](namespacenn_1_1cfg.md) <br> |
| namespace | [**codec**](namespacenn_1_1codec.md) <br> |
| namespace | [**dbg**](namespacenn_1_1dbg.md) <br> |
| namespace | [**err**](namespacenn_1_1err.md) <br> |
| namespace | [**fnd**](namespacenn_1_1fnd.md) <br> |
| namespace | [**fs**](namespacenn_1_1fs.md) <br> |
| namespace | [**fslow**](namespacenn_1_1fslow.md) <br> |
| namespace | [**hid**](namespacenn_1_1hid.md) <br> |
| namespace | [**math**](namespacenn_1_1math.md) <br> |
| namespace | [**ndm**](namespacenn_1_1ndm.md) <br> |
| namespace | [**nstd**](namespacenn_1_1nstd.md) <br> |
| namespace | [**os**](namespacenn_1_1os.md) <br> |
| namespace | [**srv**](namespacenn_1_1srv.md) <br> |
| namespace | [**svc**](namespacenn_1_1svc.md) <br> |
| namespace | [**util**](namespacenn_1_1util.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| struct | [**ConstRange**](structnn_1_1_const_range.md) &lt;TLevel, TSummary, TModule, TDescription, A, B&gt;<br> |
| struct | [**Const\_LM**](structnn_1_1_const___l_m.md) &lt;TLevel, TModule&gt;<br> |
| struct | [**Const\_LSM**](structnn_1_1_const___l_s_m.md) &lt;TLevel, TSummary, TModule&gt;<br> |
| class | [**Handle**](classnn_1_1_handle.md) <br> |
| struct | [**ProductInfo**](structnn_1_1_product_info.md) <br> |
| class | [**Result**](classnn_1_1_result.md) <br> |
| class | [**WithInitialize**](classnn_1_1_with_initialize.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**bit64**](types_8h.md#typedef-bit64) | [**ProgramID**](#typedef-programid)  <br> |
| typedef void(\* | [**nnResultHandlerImpl**](#typedef-nnresulthandlerimpl)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**NN\_RESULT\_DEF\_CONST**](#function-nn_result_def_const) (ResultSuccess, Result::LEVEL\_SUCCESS, Result::SUMMARY\_SUCCESS, Result::MODULE\_COMMON, Result::DESCRIPTION\_SUCCESS) <br> |
|   | [**\_NN\_RESULT\_MAKE\_TYPE**](#function-_nn_result_make_type) (Info, INFO) <br> |
|   | [**\_NN\_RESULT\_MAKE\_TYPE**](#function-_nn_result_make_type) (Fatal, FATAL) <br> |
|   | [**\_NN\_RESULT\_MAKE\_TYPE**](#function-_nn_result_make_type) (Reset, RESET) <br> |
|   | [**\_NN\_RESULT\_MAKE\_TYPE**](#function-_nn_result_make_type) (Reinit, REINIT) <br> |
|   | [**\_NN\_RESULT\_MAKE\_TYPE**](#function-_nn_result_make_type) (Usage, USAGE) <br> |
|   | [**\_NN\_RESULT\_MAKE\_TYPE**](#function-_nn_result_make_type) (Permanent, PERMANENT) <br> |
|   | [**\_NN\_RESULT\_MAKE\_TYPE**](#function-_nn_result_make_type) (Temporary, TEMPORARY) <br> |
|   | [**\_NN\_RESULT\_MAKE\_TYPE**](#function-_nn_result_make_type) (Status, STATUS) <br> |
|  int | [**nnResultFailureHandler**](#function-nnresultfailurehandler) ([**nnResult**](structnn_result.md) result, const char \* filename, int lineno, const char \* fmt, ...) <br> |
|  int | [**nnResultPanicHandler**](#function-nnresultpanichandler) ([**nnResult**](structnn_result.md) result, const char \* filename, int lineno, const char \* fmt, ...) <br> |
|  int | [**nnResultTFailureHandler**](#function-nnresulttfailurehandler) ([**nnResult**](structnn_result.md) result, const char \* filename, int lineno, const char \* fmt, ...) <br> |
|  int | [**nnResultTPanicHandler**](#function-nnresulttpanichandler) ([**nnResult**](structnn_result.md) result, const char \* filename, int lineno, const char \* fmt, ...) <br> |




























## Public Types Documentation




### typedef ProgramID 

```C++
typedef bit64 nn::ProgramID;
```




<hr>



### typedef nnResultHandlerImpl 

```C++
typedef void(* nn::nnResultHandlerImpl) (nnResult result, const char *filename, int lineno, const char *fmt, va_list vlist);
```




<hr>
## Public Functions Documentation




### function NN\_RESULT\_DEF\_CONST 

```C++
nn::NN_RESULT_DEF_CONST (
    ResultSuccess,
    Result::LEVEL_SUCCESS,
    Result::SUMMARY_SUCCESS,
    Result::MODULE_COMMON,
    Result::DESCRIPTION_SUCCESS
) 
```




<hr>



### function \_NN\_RESULT\_MAKE\_TYPE 

```C++
nn::_NN_RESULT_MAKE_TYPE (
    Info,
    INFO
) 
```




<hr>



### function \_NN\_RESULT\_MAKE\_TYPE 

```C++
nn::_NN_RESULT_MAKE_TYPE (
    Fatal,
    FATAL
) 
```




<hr>



### function \_NN\_RESULT\_MAKE\_TYPE 

```C++
nn::_NN_RESULT_MAKE_TYPE (
    Reset,
    RESET
) 
```




<hr>



### function \_NN\_RESULT\_MAKE\_TYPE 

```C++
nn::_NN_RESULT_MAKE_TYPE (
    Reinit,
    REINIT
) 
```




<hr>



### function \_NN\_RESULT\_MAKE\_TYPE 

```C++
nn::_NN_RESULT_MAKE_TYPE (
    Usage,
    USAGE
) 
```




<hr>



### function \_NN\_RESULT\_MAKE\_TYPE 

```C++
nn::_NN_RESULT_MAKE_TYPE (
    Permanent,
    PERMANENT
) 
```




<hr>



### function \_NN\_RESULT\_MAKE\_TYPE 

```C++
nn::_NN_RESULT_MAKE_TYPE (
    Temporary,
    TEMPORARY
) 
```




<hr>



### function \_NN\_RESULT\_MAKE\_TYPE 

```C++
nn::_NN_RESULT_MAKE_TYPE (
    Status,
    STATUS
) 
```




<hr>



### function nnResultFailureHandler 

```C++
int nn::nnResultFailureHandler (
    nnResult result,
    const char * filename,
    int lineno,
    const char * fmt,
    ...
) 
```




<hr>



### function nnResultPanicHandler 

```C++
int nn::nnResultPanicHandler (
    nnResult result,
    const char * filename,
    int lineno,
    const char * fmt,
    ...
) 
```




<hr>



### function nnResultTFailureHandler 

```C++
int nn::nnResultTFailureHandler (
    nnResult result,
    const char * filename,
    int lineno,
    const char * fmt,
    ...
) 
```




<hr>



### function nnResultTPanicHandler 

```C++
int nn::nnResultTPanicHandler (
    nnResult result,
    const char * filename,
    int lineno,
    const char * fmt,
    ...
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/applet/CTR/applet_Parameters.h`

