

# Struct nn::cfg::CTR::ParentalControlInfo



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**cfg**](namespacenn_1_1cfg.md) **>** [**CTR**](namespacenn_1_1cfg_1_1_c_t_r.md) **>** [**ParentalControlInfo**](structnn_1_1cfg_1_1_c_t_r_1_1_parental_control_info.md)





* `#include <cfg_ParentalControl.h>`





















## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**ParentalControlFlags**](structnn_1_1cfg_1_1_c_t_r_1_1_parental_control_flags.md) | [**flags**](#variable-flags)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**ogn**](#variable-ogn)  <br> |
|  char | [**password**](#variable-password)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**ratingAge**](#variable-ratingage)  <br> |
|  [**u32**](types_8h.md#typedef-u32) | [**rsv1**](#variable-rsv1)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**rsv2**](#variable-rsv2)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**rsv3**](#variable-rsv3)  <br> |
|  wchar\_t | [**secretAnswer**](#variable-secretanswer)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**secretAnswerLength**](#variable-secretanswerlength)  <br> |
|  [**u8**](types_8h.md#typedef-u8) | [**secretQuestionID**](#variable-secretquestionid)  <br> |












































## Public Attributes Documentation




### variable flags 

```C++
ParentalControlFlags nn::cfg::CTR::ParentalControlInfo::flags;
```




<hr>



### variable ogn 

```C++
u8 nn::cfg::CTR::ParentalControlInfo::ogn;
```




<hr>



### variable password 

```C++
char nn::cfg::CTR::ParentalControlInfo::password[5];
```




<hr>



### variable ratingAge 

```C++
u8 nn::cfg::CTR::ParentalControlInfo::ratingAge;
```




<hr>



### variable rsv1 

```C++
u32 nn::cfg::CTR::ParentalControlInfo::rsv1;
```




<hr>



### variable rsv2 

```C++
u8 nn::cfg::CTR::ParentalControlInfo::rsv2[3];
```




<hr>



### variable rsv3 

```C++
u8 nn::cfg::CTR::ParentalControlInfo::rsv3[42];
```




<hr>



### variable secretAnswer 

```C++
wchar_t nn::cfg::CTR::ParentalControlInfo::secretAnswer[65];
```




<hr>



### variable secretAnswerLength 

```C++
u8 nn::cfg::CTR::ParentalControlInfo::secretAnswerLength;
```




<hr>



### variable secretQuestionID 

```C++
u8 nn::cfg::CTR::ParentalControlInfo::secretQuestionID;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/cfg/CTR/cfg_ParentalControl.h`

