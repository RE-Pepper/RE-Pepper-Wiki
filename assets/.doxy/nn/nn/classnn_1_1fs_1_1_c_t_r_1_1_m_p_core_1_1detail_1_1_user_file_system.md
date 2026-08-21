

# Class nn::fs::CTR::MPCore::detail::UserFileSystem



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fs**](namespacenn_1_1fs.md) **>** [**CTR**](namespacenn_1_1fs_1_1_c_t_r.md) **>** [**MPCore**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md) **>** [**detail**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail.md) **>** [**UserFileSystem**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md)





* `#include <fs_UserFileSystem.h>`





Inherited by the following classes: [nn::fs::detail::FileSystemBaseImpl](classnn_1_1fs_1_1detail_1_1_file_system_base_impl.md)


































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**CloseDirectory**](#function-closedirectory) (void \*) <br> |
|  void | [**CloseFile**](#function-closefile) (void \* p) <br> |
|  void | [**DetachHandle**](#function-detachhandle) (void \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**DuplicateHandleForFile**](#function-duplicatehandleforfile) ([**Handle**](classnn_1_1_handle.md) \* pOut, void \*, [**s64**](types_8h.md#typedef-s64), [**s64**](types_8h.md#typedef-s64)) <br> |
|  void | [**Finalize**](#function-finalize) () <br> |
|  [**Handle**](classnn_1_1_handle.md) | [**GetFileHandle**](#function-getfilehandle) (void \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**Initialize**](#function-initialize) ([**Handle**](classnn_1_1_handle.md) handle) <br> |
|  void \*\* | [**OpenDirect**](#function-opendirect-12) ([**Handle**](classnn_1_1_handle.md) handle) <br> |
|  void | [**OpenDirect**](#function-opendirect-22) (void \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryCreateDirectory**](#function-trycreatedirectory) (const wchar\_t \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryCreateDirectoryRaw**](#function-trycreatedirectoryraw) ([**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryCreateFile**](#function-trycreatefile) (const wchar\_t \*, [**s64**](types_8h.md#typedef-s64)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryDeleteDirectory**](#function-trydeletedirectory) (const wchar\_t \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryDeleteDirectoryRaw**](#function-trydeletedirectoryraw) ([**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryDeleteDirectoryRecursively**](#function-trydeletedirectoryrecursively) (const wchar\_t \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryDeleteDirectoryRecursivelyRaw**](#function-trydeletedirectoryrecursivelyraw) ([**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryDeleteFile**](#function-trydeletefile) (const wchar\_t \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryDeleteFileRaw**](#function-trydeletefileraw) ([**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryFlush**](#function-tryflush) (void \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryGetFileSize**](#function-trygetfilesize) ([**s64**](types_8h.md#typedef-s64) \*, const void \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryOpenDirectory**](#function-tryopendirectory) (void \*\*, const wchar\_t \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryOpenDirectoryRaw**](#function-tryopendirectoryraw) (void \*\*, [**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryOpenFile**](#function-tryopenfile) (void \*\*, const wchar\_t \*, [**bit32**](types_8h.md#typedef-bit32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryOpenFileRaw**](#function-tryopenfileraw) (void \*\*, [**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &, [**bit32**](types_8h.md#typedef-bit32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryOpenFileRawDirectly**](#function-tryopenfilerawdirectly) (void \*\*, [**bit32**](types_8h.md#typedef-bit32), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &, const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &, [**bit32**](types_8h.md#typedef-bit32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryReadDirectory**](#function-tryreaddirectory) ([**s32**](types_8h.md#typedef-s32) \*, void \*, class [**DirectoryEntry**](structnn_1_1fs_1_1_directory_entry.md) \*, [**s32**](types_8h.md#typedef-s32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryReadFile**](#function-tryreadfile) ([**s32**](types_8h.md#typedef-s32) \*, void \*, [**s64**](types_8h.md#typedef-s64), void \*, size\_t) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryRenameDirectory**](#function-tryrenamedirectory) (const wchar\_t \*, const wchar\_t \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryRenameDirectoryRaw**](#function-tryrenamedirectoryraw) ([**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &, [**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryRenameFile**](#function-tryrenamefile) (const wchar\_t \*, const wchar\_t \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryRenameFileRaw**](#function-tryrenamefileraw) ([**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &, [**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TrySetFileSize**](#function-trysetfilesize) (void \*, [**s64**](types_8h.md#typedef-s64)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryWriteFile**](#function-trywritefile) ([**s32**](types_8h.md#typedef-s32) \*, void \*, [**s64**](types_8h.md#typedef-s64), const void \*, size\_t, bool) <br> |


























## Public Static Functions Documentation




### function CloseDirectory 

```C++
static void nn::fs::CTR::MPCore::detail::UserFileSystem::CloseDirectory (
    void *
) 
```




<hr>



### function CloseFile 

```C++
static void nn::fs::CTR::MPCore::detail::UserFileSystem::CloseFile (
    void * p
) 
```




<hr>



### function DetachHandle 

```C++
static void nn::fs::CTR::MPCore::detail::UserFileSystem::DetachHandle (
    void *
) 
```




<hr>



### function DuplicateHandleForFile 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::DuplicateHandleForFile (
    Handle * pOut,
    void *,
    s64,
    s64
) 
```




<hr>



### function Finalize 

```C++
static void nn::fs::CTR::MPCore::detail::UserFileSystem::Finalize () 
```




<hr>



### function GetFileHandle 

```C++
static Handle nn::fs::CTR::MPCore::detail::UserFileSystem::GetFileHandle (
    void *
) 
```




<hr>



### function Initialize 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::Initialize (
    Handle handle
) 
```




<hr>



### function OpenDirect [1/2]

```C++
static void ** nn::fs::CTR::MPCore::detail::UserFileSystem::OpenDirect (
    Handle handle
) 
```




<hr>



### function OpenDirect [2/2]

```C++
static void nn::fs::CTR::MPCore::detail::UserFileSystem::OpenDirect (
    void *
) 
```




<hr>



### function TryCreateDirectory 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryCreateDirectory (
    const wchar_t *
) 
```




<hr>



### function TryCreateDirectoryRaw 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryCreateDirectoryRaw (
    ArchiveHandle,
    const Path &
) 
```




<hr>



### function TryCreateFile 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryCreateFile (
    const wchar_t *,
    s64
) 
```




<hr>



### function TryDeleteDirectory 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryDeleteDirectory (
    const wchar_t *
) 
```




<hr>



### function TryDeleteDirectoryRaw 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryDeleteDirectoryRaw (
    ArchiveHandle,
    const Path &
) 
```




<hr>



### function TryDeleteDirectoryRecursively 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryDeleteDirectoryRecursively (
    const wchar_t *
) 
```




<hr>



### function TryDeleteDirectoryRecursivelyRaw 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryDeleteDirectoryRecursivelyRaw (
    ArchiveHandle,
    const Path &
) 
```




<hr>



### function TryDeleteFile 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryDeleteFile (
    const wchar_t *
) 
```




<hr>



### function TryDeleteFileRaw 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryDeleteFileRaw (
    ArchiveHandle,
    const Path &
) 
```




<hr>



### function TryFlush 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryFlush (
    void *
) 
```




<hr>



### function TryGetFileSize 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryGetFileSize (
    s64 *,
    const void *
) 
```




<hr>



### function TryOpenDirectory 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryOpenDirectory (
    void **,
    const wchar_t *
) 
```




<hr>



### function TryOpenDirectoryRaw 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryOpenDirectoryRaw (
    void **,
    ArchiveHandle,
    const Path &
) 
```




<hr>



### function TryOpenFile 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryOpenFile (
    void **,
    const wchar_t *,
    bit32
) 
```




<hr>



### function TryOpenFileRaw 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryOpenFileRaw (
    void **,
    ArchiveHandle,
    const Path &,
    bit32
) 
```




<hr>



### function TryOpenFileRawDirectly 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryOpenFileRawDirectly (
    void **,
    bit32,
    const Path &,
    const Path &,
    bit32
) 
```




<hr>



### function TryReadDirectory 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryReadDirectory (
    s32 *,
    void *,
    class DirectoryEntry *,
    s32
) 
```




<hr>



### function TryReadFile 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryReadFile (
    s32 *,
    void *,
    s64,
    void *,
    size_t
) 
```




<hr>



### function TryRenameDirectory 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryRenameDirectory (
    const wchar_t *,
    const wchar_t *
) 
```




<hr>



### function TryRenameDirectoryRaw 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryRenameDirectoryRaw (
    ArchiveHandle,
    const Path &,
    ArchiveHandle,
    const Path &
) 
```




<hr>



### function TryRenameFile 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryRenameFile (
    const wchar_t *,
    const wchar_t *
) 
```




<hr>



### function TryRenameFileRaw 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryRenameFileRaw (
    ArchiveHandle,
    const Path &,
    ArchiveHandle,
    const Path &
) 
```




<hr>



### function TrySetFileSize 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TrySetFileSize (
    void *,
    s64
) 
```




<hr>



### function TryWriteFile 

```C++
static Result nn::fs::CTR::MPCore::detail::UserFileSystem::TryWriteFile (
    s32 *,
    void *,
    s64,
    const void *,
    size_t,
    bool
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fs/CTR/MPCore/fs_UserFileSystem.h`

