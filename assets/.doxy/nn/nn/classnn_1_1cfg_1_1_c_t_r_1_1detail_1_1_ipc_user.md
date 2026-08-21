

# Class nn::cfg::CTR::detail::IpcUser



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**cfg**](namespacenn_1_1cfg.md) **>** [**CTR**](namespacenn_1_1cfg_1_1_c_t_r.md) **>** [**detail**](namespacenn_1_1cfg_1_1_c_t_r_1_1detail.md) **>** [**IpcUser**](classnn_1_1cfg_1_1_c_t_r_1_1detail_1_1_ipc_user.md)





* `#include <cfg_IpcUser.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**Result**](classnn_1_1_result.md) | [**GetConfig**](#function-getconfig) (void \* pData, size\_t size, [**bit32**](types_8h.md#typedef-bit32) key) const<br> |
|  [**Result**](classnn_1_1_result.md) | [**GetRegion**](#function-getregion) ([**CfgRegionCode**](namespacenn_1_1cfg_1_1_c_t_r.md#enum-cfgregioncode) \*) const<br> |
|  [**Result**](classnn_1_1_result.md) | [**GetTransferableId**](#function-gettransferableid) ([**bit32**](types_8h.md#typedef-bit32), [**bit64**](types_8h.md#typedef-bit64) \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**IsCoppacsSupported**](#function-iscoppacssupported) (bool \*) <br> |




























## Public Functions Documentation




### function GetConfig 

```C++
Result nn::cfg::CTR::detail::IpcUser::GetConfig (
    void * pData,
    size_t size,
    bit32 key
) const
```




<hr>



### function GetRegion 

```C++
Result nn::cfg::CTR::detail::IpcUser::GetRegion (
    CfgRegionCode *
) const
```




<hr>



### function GetTransferableId 

```C++
Result nn::cfg::CTR::detail::IpcUser::GetTransferableId (
    bit32,
    bit64 *
) 
```




<hr>



### function IsCoppacsSupported 

```C++
Result nn::cfg::CTR::detail::IpcUser::IsCoppacsSupported (
    bool *
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/cfg/CTR/cfg_IpcUser.h`

