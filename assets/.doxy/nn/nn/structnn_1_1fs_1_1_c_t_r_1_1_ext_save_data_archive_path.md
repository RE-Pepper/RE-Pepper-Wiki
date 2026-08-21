

# Struct nn::fs::CTR::ExtSaveDataArchivePath



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fs**](namespacenn_1_1fs.md) **>** [**CTR**](namespacenn_1_1fs_1_1_c_t_r.md) **>** [**ExtSaveDataArchivePath**](structnn_1_1fs_1_1_c_t_r_1_1_ext_save_data_archive_path.md)





* `#include <fs_ArchiveTypes.h>`





















## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**util::Int64**](classnn_1_1util_1_1_int64.md)&lt; [**bit64**](types_8h.md#typedef-bit64) &gt; | [**extSaveDataId**](#variable-extsavedataid)  <br> |
|  [**util::SizedEnum4**](structnn_1_1util_1_1_sized_enum4.md)&lt; [**MediaType**](namespacenn_1_1fs.md#enum-mediatype) &gt; | [**mediaType**](#variable-mediatype)  <br> |


















## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**ExtSaveDataArchivePath**](structnn_1_1fs_1_1_c_t_r_1_1_ext_save_data_archive_path.md) | [**Make**](#function-make) ([**MediaType**](namespacenn_1_1fs.md#enum-mediatype) mediaType, [**ExtSaveDataId**](namespacenn_1_1fs.md#typedef-extsavedataid) extSaveDataId) <br> |


























## Public Attributes Documentation




### variable extSaveDataId 

```C++
util::Int64<bit64> nn::fs::CTR::ExtSaveDataArchivePath::extSaveDataId;
```




<hr>



### variable mediaType 

```C++
util::SizedEnum4<MediaType> nn::fs::CTR::ExtSaveDataArchivePath::mediaType;
```




<hr>
## Public Static Functions Documentation




### function Make 

```C++
static inline ExtSaveDataArchivePath nn::fs::CTR::ExtSaveDataArchivePath::Make (
    MediaType mediaType,
    ExtSaveDataId extSaveDataId
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fs/CTR/fs_ArchiveTypes.h`

