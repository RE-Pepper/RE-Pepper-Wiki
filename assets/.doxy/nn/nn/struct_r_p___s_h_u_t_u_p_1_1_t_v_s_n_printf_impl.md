

# Struct RP\_SHUTUP::TVSNPrintfImpl

**template &lt;[**typename**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md) Type&gt;**



[**ClassList**](annotated.md) **>** [**RP\_SHUTUP**](namespace_r_p___s_h_u_t_u_p.md) **>** [**TVSNPrintfImpl**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md)




















## Classes

| Type | Name |
| ---: | :--- |
| struct | [**dst\_string**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl_1_1dst__string.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef Type::char\_type | [**CharT**](#typedef-chart)  <br> |






















## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**s32**](types_8h.md#typedef-s32) | [**TVSNPrintf**](#function-tvsnprintf) ([**char**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md) \* dst, [**size\_t**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md) len, [**const**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md) [**CharT**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md#typedef-chart) \* fmt, [**va\_list**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md) vlist) <br> |
|  [**void**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md) | [**string\_fill\_char**](#function-string_fill_char) ([**dst\_string**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl_1_1dst__string.md) \* p, [**CharT**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md#typedef-chart) c, [**int**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md) n) <br> |
|  [**void**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md) | [**string\_put\_char**](#function-string_put_char) ([**dst\_string**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl_1_1dst__string.md) \* p, [**CharT**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md#typedef-chart) c) <br> |
|  [**void**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md) | [**string\_put\_string**](#function-string_put_string) ([**dst\_string**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl_1_1dst__string.md) \* p, [**const**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md) [**CharT**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md#typedef-chart) \* s, [**int**](struct_r_p___s_h_u_t_u_p_1_1_t_v_s_n_printf_impl.md) n) <br> |


























## Public Types Documentation




### typedef CharT 

```C++
typedef Type::char_type RP_SHUTUP::TVSNPrintfImpl< Type >::CharT;
```




<hr>
## Public Static Functions Documentation




### function TVSNPrintf 

```C++
static inline s32 RP_SHUTUP::TVSNPrintfImpl::TVSNPrintf (
    char * dst,
    size_t len,
    const  CharT * fmt,
    va_list vlist
) 
```




<hr>



### function string\_fill\_char 

```C++
static inline void RP_SHUTUP::TVSNPrintfImpl::string_fill_char (
    dst_string * p,
    CharT c,
    int n
) 
```




<hr>



### function string\_put\_char 

```C++
static inline void RP_SHUTUP::TVSNPrintfImpl::string_put_char (
    dst_string * p,
    CharT c
) 
```




<hr>



### function string\_put\_string 

```C++
static inline void RP_SHUTUP::TVSNPrintfImpl::string_put_string (
    dst_string * p,
    const  CharT * s,
    int n
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/sources/libraries/nstd/nstd_Printf.cpp`

