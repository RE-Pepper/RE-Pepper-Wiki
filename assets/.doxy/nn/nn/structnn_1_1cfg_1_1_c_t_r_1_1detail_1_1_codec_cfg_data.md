

# Struct nn::cfg::CTR::detail::CodecCfgData



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**cfg**](namespacenn_1_1cfg.md) **>** [**CTR**](namespacenn_1_1cfg_1_1_c_t_r.md) **>** [**detail**](namespacenn_1_1cfg_1_1_c_t_r_1_1detail.md) **>** [**CodecCfgData**](structnn_1_1cfg_1_1_c_t_r_1_1detail_1_1_codec_cfg_data.md)





* `#include <cfg_DataStructures.h>`





















## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**AnalogInterfaceParam**](structnn_1_1cfg_1_1_c_t_r_1_1detail_1_1_analog_interface_param.md) | [**AnalogInterfaceParam**](#variable-analoginterfaceparam)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**analogVolumeHP**](#variable-analogvolumehp)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**analogVolumeSP**](#variable-analogvolumesp)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**driverGainHP**](#variable-drivergainhp)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**driverGainSP**](#variable-drivergainsp)  <br> |
|  [**codec::CTR::IirFilterParam**](structnn_1_1codec_1_1_c_t_r_1_1_iir_filter_param.md) | [**filterFree**](#variable-filterfree)  <br> |
|  [**codec::CTR::IirFilterParamEQ**](structnn_1_1codec_1_1_c_t_r_1_1_iir_filter_param_e_q.md) | [**filterHp32**](#variable-filterhp32)  <br> |
|  [**codec::CTR::IirFilterParamEQ**](structnn_1_1codec_1_1_c_t_r_1_1_iir_filter_param_e_q.md) | [**filterHp47**](#variable-filterhp47)  <br> |
|  [**codec::CTR::IirFilterParam**](structnn_1_1codec_1_1_c_t_r_1_1_iir_filter_param.md) | [**filterMic32**](#variable-filtermic32)  <br> |
|  [**codec::CTR::IirFilterParam**](structnn_1_1codec_1_1_c_t_r_1_1_iir_filter_param.md) | [**filterMic47**](#variable-filtermic47)  <br> |
|  [**codec::CTR::IirFilterParamEQ**](structnn_1_1codec_1_1_c_t_r_1_1_iir_filter_param_e_q.md) | [**filterSp32**](#variable-filtersp32)  <br> |
|  [**codec::CTR::IirFilterParamEQ**](structnn_1_1codec_1_1_c_t_r_1_1_iir_filter_param_e_q.md) | [**filterSp47**](#variable-filtersp47)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**micBias**](#variable-micbias)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**micGainCalibrateParam**](#variable-micgaincalibrateparam)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**pad**](#variable-pad)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**quickCharge**](#variable-quickcharge)  <br> |
|  [**s8**](types_8h.md#typedef-s8) | [**shutterVolume1**](#variable-shuttervolume1)  <br> |
|  [**s8**](types_8h.md#typedef-s8) | [**shutterVolume2**](#variable-shuttervolume2)  <br> |












































## Public Attributes Documentation




### variable AnalogInterfaceParam 

```C++
AnalogInterfaceParam nn::cfg::CTR::detail::CodecCfgData::AnalogInterfaceParam;
```




<hr>



### variable analogVolumeHP 

```C++
u8 nn::cfg::CTR::detail::CodecCfgData::analogVolumeHP;
```




<hr>



### variable analogVolumeSP 

```C++
u8 nn::cfg::CTR::detail::CodecCfgData::analogVolumeSP;
```




<hr>



### variable driverGainHP 

```C++
u8 nn::cfg::CTR::detail::CodecCfgData::driverGainHP;
```




<hr>



### variable driverGainSP 

```C++
u8 nn::cfg::CTR::detail::CodecCfgData::driverGainSP;
```




<hr>



### variable filterFree 

```C++
codec::CTR::IirFilterParam nn::cfg::CTR::detail::CodecCfgData::filterFree;
```




<hr>



### variable filterHp32 

```C++
codec::CTR::IirFilterParamEQ nn::cfg::CTR::detail::CodecCfgData::filterHp32;
```




<hr>



### variable filterHp47 

```C++
codec::CTR::IirFilterParamEQ nn::cfg::CTR::detail::CodecCfgData::filterHp47;
```




<hr>



### variable filterMic32 

```C++
codec::CTR::IirFilterParam nn::cfg::CTR::detail::CodecCfgData::filterMic32;
```




<hr>



### variable filterMic47 

```C++
codec::CTR::IirFilterParam nn::cfg::CTR::detail::CodecCfgData::filterMic47;
```




<hr>



### variable filterSp32 

```C++
codec::CTR::IirFilterParamEQ nn::cfg::CTR::detail::CodecCfgData::filterSp32;
```




<hr>



### variable filterSp47 

```C++
codec::CTR::IirFilterParamEQ nn::cfg::CTR::detail::CodecCfgData::filterSp47;
```




<hr>



### variable micBias 

```C++
u8 nn::cfg::CTR::detail::CodecCfgData::micBias;
```




<hr>



### variable micGainCalibrateParam 

```C++
u8 nn::cfg::CTR::detail::CodecCfgData::micGainCalibrateParam;
```




<hr>



### variable pad 

```C++
u8 nn::cfg::CTR::detail::CodecCfgData::pad[3];
```




<hr>



### variable quickCharge 

```C++
u8 nn::cfg::CTR::detail::CodecCfgData::quickCharge;
```




<hr>



### variable shutterVolume1 

```C++
s8 nn::cfg::CTR::detail::CodecCfgData::shutterVolume1;
```




<hr>



### variable shutterVolume2 

```C++
s8 nn::cfg::CTR::detail::CodecCfgData::shutterVolume2;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/cfg/CTR/detail/cfg_DataStructures.h`

