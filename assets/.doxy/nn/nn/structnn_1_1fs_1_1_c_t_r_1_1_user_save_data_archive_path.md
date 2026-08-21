

# Struct nn::fs::CTR::UserSaveDataArchivePath



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fs**](namespacenn_1_1fs.md) **>** [**CTR**](namespacenn_1_1fs_1_1_c_t_r.md) **>** [**UserSaveDataArchivePath**](structnn_1_1fs_1_1_c_t_r_1_1_user_save_data_archive_path.md)





* `#include <fs_ArchiveTypes.h>`





















## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**util::SizedEnum4**](structnn_1_1util_1_1_sized_enum4.md)&lt; [**MediaType**](namespacenn_1_1fs.md#enum-mediatype) &gt; | [**mediaType**](#variable-mediatype)  <br> |
|  [**util::Int64**](classnn_1_1util_1_1_int64.md)&lt; [**bit64**](types_8h.md#typedef-bit64) &gt; | [**titleId**](#variable-titleid)  <br> |


















## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**UserSaveDataArchivePath**](structnn_1_1fs_1_1_c_t_r_1_1_user_save_data_archive_path.md) | [**Make**](#function-make) ([**MediaType**](namespacenn_1_1fs.md#enum-mediatype) mediaType, [**TitleId**](namespacenn_1_1fs.md#typedef-titleid) id) <br> |


























## Public Attributes Documentation




### variable mediaType 

```C++
util::SizedEnum4<MediaType> nn::fs::CTR::UserSaveDataArchivePath::mediaType;
```




<hr>



### variable titleId 

```C++
util::Int64<bit64> nn::fs::CTR::UserSaveDataArchivePath::titleId;
```




<hr>
## Public Static Functions Documentation




### function Make 

```C++
static inline UserSaveDataArchivePath nn::fs::CTR::UserSaveDataArchivePath::Make (
    MediaType mediaType,
    TitleId id
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fs/CTR/fs_ArchiveTypes.h`

