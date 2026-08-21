

# Struct nn::fs::TitleDataSpecifier



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fs**](namespacenn_1_1fs.md) **>** [**TitleDataSpecifier**](structnn_1_1fs_1_1_title_data_specifier.md)





* `#include <fs_ParametersForSystem.h>`





















## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**TitleId**](namespacenn_1_1fs.md#typedef-titleid) | [**id**](#variable-id)  <br> |
|  [**util::SizedEnum1**](structnn_1_1util_1_1_sized_enum1.md)&lt; [**MediaType**](namespacenn_1_1fs.md#enum-mediatype) &gt; | [**media**](#variable-media)  <br> |
|  int | [**unk0**](#variable-unk0)  <br> |
|  int | [**unk1**](#variable-unk1)  <br> |


















## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**TitleDataSpecifier**](structnn_1_1fs_1_1_title_data_specifier.md) | [**Make**](#function-make) ([**MediaType**](namespacenn_1_1fs.md#enum-mediatype) type, [**TitleId**](namespacenn_1_1fs.md#typedef-titleid) id) <br> |


























## Public Attributes Documentation




### variable id 

```C++
TitleId nn::fs::TitleDataSpecifier::id;
```




<hr>



### variable media 

```C++
util::SizedEnum1<MediaType> nn::fs::TitleDataSpecifier::media;
```




<hr>



### variable unk0 

```C++
int nn::fs::TitleDataSpecifier::unk0;
```




<hr>



### variable unk1 

```C++
int nn::fs::TitleDataSpecifier::unk1;
```




<hr>
## Public Static Functions Documentation




### function Make 

```C++
static inline TitleDataSpecifier nn::fs::TitleDataSpecifier::Make (
    MediaType type,
    TitleId id
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fs/fs_ParametersForSystem.h`

