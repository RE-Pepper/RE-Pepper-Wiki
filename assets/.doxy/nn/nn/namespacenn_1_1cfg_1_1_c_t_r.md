

# Namespace nn::cfg::CTR



[**Namespace List**](namespaces.md) **>** [**nn**](namespacenn.md) **>** [**cfg**](namespacenn_1_1cfg.md) **>** [**CTR**](namespacenn_1_1cfg_1_1_c_t_r.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**detail**](namespacenn_1_1cfg_1_1_c_t_r_1_1detail.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| struct | [**Birthday**](structnn_1_1cfg_1_1_c_t_r_1_1_birthday.md) <br> |
| struct | [**ParentalControlFlags**](structnn_1_1cfg_1_1_c_t_r_1_1_parental_control_flags.md) <br> |
| struct | [**ParentalControlInfo**](structnn_1_1cfg_1_1_c_t_r_1_1_parental_control_info.md) <br> |
| struct | [**SimpleAddress**](structnn_1_1cfg_1_1_c_t_r_1_1_simple_address.md) <br> |
| struct | [**UserName**](structnn_1_1cfg_1_1_c_t_r_1_1_user_name.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| enum  | [**CfgLanguageCode**](#enum-cfglanguagecode)  <br> |
| enum  | [**CfgRegionCode**](#enum-cfgregioncode)  <br> |
| enum  | [**CfgSoundOutputMode**](#enum-cfgsoundoutputmode)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**Initialize**](#function-initialize) () <br> |




























## Public Types Documentation




### enum CfgLanguageCode 

```C++
enum nn::cfg::CTR::CfgLanguageCode {
    CFG_LANGUAGE_JAPANESE = 0,
    CFG_LANGUAGE_ENGLISH = 1,
    CFG_LANGUAGE_FRENCH = 2,
    CFG_LANGUAGE_GERMAN = 3,
    CFG_LANGUAGE_ITALIAN = 4,
    CFG_LANGUAGE_SPANISH = 5,
    CFG_LANGUAGE_SIMP_CHINESE = 6,
    CFG_LANGUAGE_KOREAN = 7,
    CFG_LANGUAGE_DUTCH = 8,
    CFG_LANGUAGE_PORTUGUESE = 9,
    CFG_LANGUAGE_RUSSIAN = 10,
    CFG_LANGUAGE_TRAD_CHINESE = 11,
    CFG_LANGUAGE_CODE_MAX = 12
};
```




<hr>



### enum CfgRegionCode 

```C++
enum nn::cfg::CTR::CfgRegionCode {
    CFG_REGION_JAPAN = 0,
    CFG_REGION_AMERICA = 1,
    CFG_REGION_EUROPE = 2,
    CFG_REGION_AUSTRALIA = 3,
    CFG_REGION_CHINA = 4,
    CFG_REGION_KOREA = 5,
    CFG_REGION_TAIWAN = 6,
    CFG_REGION_MAX = 7
};
```




<hr>



### enum CfgSoundOutputMode 

```C++
enum nn::cfg::CTR::CfgSoundOutputMode {
    CFG_SOUND_OUTPUT_MODE_MONO = 0,
    CFG_SOUND_OUTPUT_MODE_STEREO = 1,
    CFG_SOUND_OUTPUT_MODE_SURROUND = 2
};
```




<hr>
## Public Functions Documentation




### function Initialize 

```C++
void nn::cfg::CTR::Initialize () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/cfg/CTR/cfg_Api.h`

