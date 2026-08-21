

# Namespace nn::fs



[**Namespace List**](namespaces.md) **>** [**nn**](namespacenn.md) **>** [**fs**](namespacenn_1_1fs.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**CTR**](namespacenn_1_1fs_1_1_c_t_r.md) <br> |
| namespace | [**detail**](namespacenn_1_1fs_1_1detail.md) <br> |
| namespace | [**ipc**](namespacenn_1_1fs_1_1ipc.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| struct | [**ArchiveResource**](structnn_1_1fs_1_1_archive_resource.md) <br> |
| struct | [**Attributes**](structnn_1_1fs_1_1_attributes.md) <br> |
| struct | [**DirectoryEntry**](structnn_1_1fs_1_1_directory_entry.md) <br> |
| struct | [**NandInfo**](structnn_1_1fs_1_1_nand_info.md) <br> |
| struct | [**SdmcSpeedInfo**](structnn_1_1fs_1_1_sdmc_speed_info.md) <br> |
| struct | [**ShortName**](structnn_1_1fs_1_1_short_name.md) <br> |
| struct | [**TitleDataSpecifier**](structnn_1_1fs_1_1_title_data_specifier.md) <br> |
| struct | [**Transaction**](structnn_1_1fs_1_1_transaction.md) <br> |
| struct | [**WriteOption**](structnn_1_1fs_1_1_write_option.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| typedef [**bit64**](types_8h.md#typedef-bit64) | [**ArchiveHandle**](#typedef-archivehandle)  <br> |
| typedef struct [**nn::fs::ArchiveResource**](structnn_1_1fs_1_1_archive_resource.md) | [**ArchiveResource**](#typedef-archiveresource)  <br> |
| enum  | [**CardSpiBaudRate**](#enum-cardspibaudrate)  <br> |
| enum  | [**CardSpiBusMode**](#enum-cardspibusmode)  <br> |
| enum  | [**CardType**](#enum-cardtype)  <br> |
| typedef enum [**nn::fs::CardType**](namespacenn_1_1fs.md#enum-cardtype) | [**CardType**](#typedef-cardtype)  <br> |
| typedef [**bit32**](types_8h.md#typedef-bit32) | [**ContentIdx**](#typedef-contentidx)  <br> |
| typedef [**bit64**](types_8h.md#typedef-bit64) | [**ExtSaveDataId**](#typedef-extsavedataid)  <br> |
| enum  | [**MediaType**](#enum-mediatype)  <br> |
| typedef struct [**nn::fs::NandInfo**](structnn_1_1fs_1_1_nand_info.md) | [**NandInfo**](#typedef-nandinfo)  <br> |
| typedef struct [**NandLog**](namespacenn_1_1fs.md#typedef-nandlog) | [**NandLog**](#typedef-nandlog)  <br> |
| enum  | [**PositionBase**](#enum-positionbase)  <br> |
| typedef struct [**nn::fs::TitleDataSpecifier**](structnn_1_1fs_1_1_title_data_specifier.md) | [**ProgramLaunchInfo**](#typedef-programlaunchinfo)  <br> |
| typedef struct [**SdmcLog**](namespacenn_1_1fs.md#typedef-sdmclog) | [**SdmcLog**](#typedef-sdmclog)  <br> |
| enum  | [**SystemMediaType**](#enum-systemmediatype)  <br> |
| typedef [**bit32**](types_8h.md#typedef-bit32) | [**SystemSaveDataId**](#typedef-systemsavedataid)  <br> |
| typedef [**bit64**](types_8h.md#typedef-bit64) | [**TitleId**](#typedef-titleid)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**ForceDisableLatencyEmulation**](#function-forcedisablelatencyemulation) () <br> |
|  void | [**Initialize**](#function-initialize) () <br> |




























## Public Types Documentation




### typedef ArchiveHandle 

```C++
typedef bit64 nn::fs::ArchiveHandle;
```




<hr>



### typedef ArchiveResource 

```C++
typedef struct nn::fs::ArchiveResource nn::fs::ArchiveResource;
```




<hr>



### enum CardSpiBaudRate 

```C++
enum nn::fs::CardSpiBaudRate {
    CARDSPI_BAUDRATE_512KHZ = 0,
    CARDSPI_BAUDRATE_1MHZ = 1,
    CARDSPI_BAUDRATE_2MHZ = 2,
    CARDSPI_BAUDRATE_4MHZ = 3,
    CARDSPI_BAUDRATE_8MHZ = 4,
    CARDSPI_BAUDRATE_16MHZ = 5
};
```




<hr>



### enum CardSpiBusMode 

```C++
enum nn::fs::CardSpiBusMode {
    CARDSPI_BUSMODE_1BIT = 0,
    CARDSPI_BUSMODE_4BIT = 1
};
```




<hr>



### enum CardType 

```C++
enum nn::fs::CardType {
    CARD_TYPE_CTR,
    CARD_TYPE_DS_TWL,
    CARD_TYPE_UNKNOWN
};
```




<hr>



### typedef CardType 

```C++
typedef enum nn::fs::CardType nn::fs::CardType;
```




<hr>



### typedef ContentIdx 

```C++
typedef bit32 nn::fs::ContentIdx;
```




<hr>



### typedef ExtSaveDataId 

```C++
typedef bit64 nn::fs::ExtSaveDataId;
```




<hr>



### enum MediaType 

```C++
enum nn::fs::MediaType {
    MEDIA_TYPE_NAND,
    MEDIA_TYPE_SDMC,
    MEDIA_TYPE_CTRCARD
};
```




<hr>



### typedef NandInfo 

```C++
typedef struct nn::fs::NandInfo nn::fs::NandInfo;
```




<hr>



### typedef NandLog 

```C++
typedef struct NandLog nn::fs::NandLog;
```




<hr>



### enum PositionBase 

```C++
enum nn::fs::PositionBase {
    POSITION_BASE_BEGIN,
    POSITION_BASE_CURRENT,
    POSITION_BASE_END
};
```




<hr>



### typedef ProgramLaunchInfo 

```C++
typedef struct nn::fs::TitleDataSpecifier nn::fs::ProgramLaunchInfo;
```




<hr>



### typedef SdmcLog 

```C++
typedef struct SdmcLog nn::fs::SdmcLog;
```




<hr>



### enum SystemMediaType 

```C++
enum nn::fs::SystemMediaType {
    SYSTEM_MEDIA_TYPE_CTR_NAND,
    SYSTEM_MEDIA_TYPE_TWL_NAND,
    SYSTEM_MEDIA_TYPE_SDMC,
    SYSTEM_MEDIA_TYPE_TWL_PHOTO
};
```




<hr>



### typedef SystemSaveDataId 

```C++
typedef bit32 nn::fs::SystemSaveDataId;
```




<hr>



### typedef TitleId 

```C++
typedef bit64 nn::fs::TitleId;
```




<hr>
## Public Functions Documentation




### function ForceDisableLatencyEmulation 

```C++
void nn::fs::ForceDisableLatencyEmulation () 
```




<hr>



### function Initialize 

```C++
void nn::fs::Initialize () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fs/CTR/fs_ArchiveTypes.h`

