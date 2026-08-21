

# Struct nn::fs::CTR::SystemSaveDataArchivePath



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fs**](namespacenn_1_1fs.md) **>** [**CTR**](namespacenn_1_1fs_1_1_c_t_r.md) **>** [**SystemSaveDataArchivePath**](structnn_1_1fs_1_1_c_t_r_1_1_system_save_data_archive_path.md)





* `#include <fs_ArchiveTypes.h>`





















## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**util::SizedEnum4**](structnn_1_1util_1_1_sized_enum4.md)&lt; [**MediaType**](namespacenn_1_1fs.md#enum-mediatype) &gt; | [**mediaType**](#variable-mediatype)  <br> |
|  [**SystemSaveDataId**](namespacenn_1_1fs.md#typedef-systemsavedataid) | [**systemSaveDataId**](#variable-systemsavedataid)  <br> |


















## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**SystemSaveDataArchivePath**](structnn_1_1fs_1_1_c_t_r_1_1_system_save_data_archive_path.md) | [**Make**](#function-make) ([**MediaType**](namespacenn_1_1fs.md#enum-mediatype) mediaType, [**SystemSaveDataId**](namespacenn_1_1fs.md#typedef-systemsavedataid) systemSaveDataId) <br> |


























## Public Attributes Documentation




### variable mediaType 

```C++
util::SizedEnum4<MediaType> nn::fs::CTR::SystemSaveDataArchivePath::mediaType;
```




<hr>



### variable systemSaveDataId 

```C++
SystemSaveDataId nn::fs::CTR::SystemSaveDataArchivePath::systemSaveDataId;
```




<hr>
## Public Static Functions Documentation




### function Make 

```C++
static inline SystemSaveDataArchivePath nn::fs::CTR::SystemSaveDataArchivePath::Make (
    MediaType mediaType,
    SystemSaveDataId systemSaveDataId
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fs/CTR/fs_ArchiveTypes.h`

