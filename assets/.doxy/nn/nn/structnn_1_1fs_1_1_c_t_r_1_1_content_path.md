

# Struct nn::fs::CTR::ContentPath



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fs**](namespacenn_1_1fs.md) **>** [**CTR**](namespacenn_1_1fs_1_1_c_t_r.md) **>** [**ContentPath**](structnn_1_1fs_1_1_c_t_r_1_1_content_path.md)





* `#include <fs_PathNamesForSystem.h>`



Inherits the following classes: [nn::fs::CTR::ExeFsSectionNames](structnn_1_1fs_1_1_c_t_r_1_1_exe_fs_section_names.md)














## Public Types

| Type | Name |
| ---: | :--- |
| enum  | [**Tag**](#enum-tag)  <br> |








## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**util::Int64**](classnn_1_1util_1_1_int64.md)&lt; [**s64**](types_8h.md#typedef-s64) &gt; | [**id**](#variable-id)  <br> |
|  [**util::SizedEnum4**](structnn_1_1util_1_1_sized_enum4.md)&lt; [**Tag**](structnn_1_1fs_1_1_c_t_r_1_1_content_path.md#enum-tag) &gt; | [**tag**](#variable-tag)  <br> |




































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**ContentPath**](structnn_1_1fs_1_1_c_t_r_1_1_content_path.md) | [**MakeExefsPath**](#function-makeexefspath) () <br> |
|  [**ContentPath**](structnn_1_1fs_1_1_c_t_r_1_1_content_path.md) | [**MakeProgramInfoPath**](#function-makeprograminfopath) () <br> |
|  [**ContentPath**](structnn_1_1fs_1_1_c_t_r_1_1_content_path.md) | [**MakeRomfsPath**](#function-makeromfspath) () <br> |
|  [**ContentPath**](structnn_1_1fs_1_1_c_t_r_1_1_content_path.md) | [**MakeSystemMenuDataPath**](#function-makesystemmenudatapath) () <br> |




















































## Public Types Documentation




### enum Tag 

```C++
enum nn::fs::CTR::ContentPath::Tag {
    TAG_ROMFS,
    TAG_EXEFS,
    TAG_SYSTEM_MENU_DATA,
    TAG_PROGRAM_INFO
};
```




<hr>
## Public Attributes Documentation




### variable id 

```C++
util::Int64<s64> nn::fs::CTR::ContentPath::id;
```




<hr>



### variable tag 

```C++
util::SizedEnum4<Tag> nn::fs::CTR::ContentPath::tag;
```




<hr>
## Public Static Functions Documentation




### function MakeExefsPath 

```C++
static inline ContentPath nn::fs::CTR::ContentPath::MakeExefsPath () 
```




<hr>



### function MakeProgramInfoPath 

```C++
static inline ContentPath nn::fs::CTR::ContentPath::MakeProgramInfoPath () 
```




<hr>



### function MakeRomfsPath 

```C++
static inline ContentPath nn::fs::CTR::ContentPath::MakeRomfsPath () 
```




<hr>



### function MakeSystemMenuDataPath 

```C++
static inline ContentPath nn::fs::CTR::ContentPath::MakeSystemMenuDataPath () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fslow/CTR/fs_PathNamesForSystem.h`

