

# Struct nn::fs::CTR::ProgramDataPath



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fs**](namespacenn_1_1fs.md) **>** [**CTR**](namespacenn_1_1fs_1_1_c_t_r.md) **>** [**ProgramDataPath**](structnn_1_1fs_1_1_c_t_r_1_1_program_data_path.md)





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
|  [**util::SizedEnum4**](structnn_1_1util_1_1_sized_enum4.md)&lt; [**Tag**](structnn_1_1fs_1_1_c_t_r_1_1_program_data_path.md#enum-tag) &gt; | [**tag**](#variable-tag)  <br> |




































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**ProgramDataPath**](structnn_1_1fs_1_1_c_t_r_1_1_program_data_path.md) | [**MakeContentDataPath**](#function-makecontentdatapath) () <br> |
|  [**ProgramDataPath**](structnn_1_1fs_1_1_c_t_r_1_1_program_data_path.md) | [**MakeExeFsPath**](#function-makeexefspath) () <br> |
|  [**ProgramDataPath**](structnn_1_1fs_1_1_c_t_r_1_1_program_data_path.md) | [**MakeRomFsPath**](#function-makeromfspath) () <br> |
|  [**ProgramDataPath**](structnn_1_1fs_1_1_c_t_r_1_1_program_data_path.md) | [**MakeSaveDataPath**](#function-makesavedatapath) () <br> |
|  [**ProgramDataPath**](structnn_1_1fs_1_1_c_t_r_1_1_program_data_path.md) | [**MakeSaveMenuDataPath**](#function-makesavemenudatapath) () <br> |




















































## Public Types Documentation




### enum Tag 

```C++
enum nn::fs::CTR::ProgramDataPath::Tag {
    TAG_ROMFS,
    TAG_EXEFS,
    TAG_SYSTEM_MENU_DATA,
    TAG_SAVE_DATA,
    TAG_CONTENT
};
```




<hr>
## Public Attributes Documentation




### variable id 

```C++
util::Int64<s64> nn::fs::CTR::ProgramDataPath::id;
```




<hr>



### variable tag 

```C++
util::SizedEnum4<Tag> nn::fs::CTR::ProgramDataPath::tag;
```




<hr>
## Public Static Functions Documentation




### function MakeContentDataPath 

```C++
static inline ProgramDataPath nn::fs::CTR::ProgramDataPath::MakeContentDataPath () 
```




<hr>



### function MakeExeFsPath 

```C++
static inline ProgramDataPath nn::fs::CTR::ProgramDataPath::MakeExeFsPath () 
```




<hr>



### function MakeRomFsPath 

```C++
static inline ProgramDataPath nn::fs::CTR::ProgramDataPath::MakeRomFsPath () 
```




<hr>



### function MakeSaveDataPath 

```C++
static inline ProgramDataPath nn::fs::CTR::ProgramDataPath::MakeSaveDataPath () 
```




<hr>



### function MakeSaveMenuDataPath 

```C++
static inline ProgramDataPath nn::fs::CTR::ProgramDataPath::MakeSaveMenuDataPath () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fslow/CTR/fs_PathNamesForSystem.h`

