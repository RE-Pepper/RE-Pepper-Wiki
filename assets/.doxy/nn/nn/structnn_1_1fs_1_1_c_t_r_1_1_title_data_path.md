

# Struct nn::fs::CTR::TitleDataPath



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fs**](namespacenn_1_1fs.md) **>** [**CTR**](namespacenn_1_1fs_1_1_c_t_r.md) **>** [**TitleDataPath**](structnn_1_1fs_1_1_c_t_r_1_1_title_data_path.md)





* `#include <fs_PathNamesForSystem.h>`



Inherits the following classes: [nn::fs::CTR::ExeFsSectionNames](structnn_1_1fs_1_1_c_t_r_1_1_exe_fs_section_names.md)














## Public Types

| Type | Name |
| ---: | :--- |
| enum  | [**Tag**](#enum-tag)  <br> |








## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**ContentIdx**](namespacenn_1_1fs.md#typedef-contentidx) | [**contentIdx**](#variable-contentidx)  <br> |
|  [**util::SizedEnum4**](structnn_1_1util_1_1_sized_enum4.md)&lt; [**Tag**](structnn_1_1fs_1_1_c_t_r_1_1_title_data_path.md#enum-tag) &gt; | [**tag**](#variable-tag)  <br> |




































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**TitleDataPath**](structnn_1_1fs_1_1_c_t_r_1_1_title_data_path.md) | [**MakeContentDataPath**](#function-makecontentdatapath) ([**ContentIdx**](namespacenn_1_1fs.md#typedef-contentidx) idx) <br> |
|  [**TitleDataPath**](structnn_1_1fs_1_1_c_t_r_1_1_title_data_path.md) | [**MakeLegacyContentPath**](#function-makelegacycontentpath) ([**ContentIdx**](namespacenn_1_1fs.md#typedef-contentidx) idx) <br> |
|  [**TitleDataPath**](structnn_1_1fs_1_1_c_t_r_1_1_title_data_path.md) | [**MakeLegacySubbannerPath**](#function-makelegacysubbannerpath) ([**ContentIdx**](namespacenn_1_1fs.md#typedef-contentidx) idx) <br> |
|  [**TitleDataPath**](structnn_1_1fs_1_1_c_t_r_1_1_title_data_path.md) | [**MakeSaveDataPath**](#function-makesavedatapath) ([**ContentIdx**](namespacenn_1_1fs.md#typedef-contentidx) idx) <br> |




















































## Public Types Documentation




### enum Tag 

```C++
enum nn::fs::CTR::TitleDataPath::Tag {
    TAG_CONTENT_FILE,
    TAG_SAVE_DATA_FILE,
    TAG_LEGACY_CONTENT_FILE,
    TAG_LEGACY_SUBBANNER_FILE
};
```




<hr>
## Public Attributes Documentation




### variable contentIdx 

```C++
ContentIdx nn::fs::CTR::TitleDataPath::contentIdx;
```




<hr>



### variable tag 

```C++
util::SizedEnum4<Tag> nn::fs::CTR::TitleDataPath::tag;
```




<hr>
## Public Static Functions Documentation




### function MakeContentDataPath 

```C++
static inline TitleDataPath nn::fs::CTR::TitleDataPath::MakeContentDataPath (
    ContentIdx idx
) 
```




<hr>



### function MakeLegacyContentPath 

```C++
static inline TitleDataPath nn::fs::CTR::TitleDataPath::MakeLegacyContentPath (
    ContentIdx idx
) 
```




<hr>



### function MakeLegacySubbannerPath 

```C++
static inline TitleDataPath nn::fs::CTR::TitleDataPath::MakeLegacySubbannerPath (
    ContentIdx idx
) 
```




<hr>



### function MakeSaveDataPath 

```C++
static inline TitleDataPath nn::fs::CTR::TitleDataPath::MakeSaveDataPath (
    ContentIdx idx
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fslow/CTR/fs_PathNamesForSystem.h`

