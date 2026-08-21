

# Class nn::fs::detail::FileSystemBaseImpl



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fs**](namespacenn_1_1fs.md) **>** [**detail**](namespacenn_1_1fs_1_1detail.md) **>** [**FileSystemBaseImpl**](classnn_1_1fs_1_1detail_1_1_file_system_base_impl.md)





* `#include <fs_FileSystemBase.h>`



Inherits the following classes: [nn::fs::CTR::MPCore::detail::UserFileSystem](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md)




























































## Public Static Functions inherited from nn::fs::CTR::MPCore::detail::UserFileSystem

See [nn::fs::CTR::MPCore::detail::UserFileSystem](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md)

| Type | Name |
| ---: | :--- |
|  void | [**CloseDirectory**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-closedirectory) (void \*) <br> |
|  void | [**CloseFile**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-closefile) (void \* p) <br> |
|  void | [**DetachHandle**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-detachhandle) (void \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**DuplicateHandleForFile**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-duplicatehandleforfile) ([**Handle**](classnn_1_1_handle.md) \* pOut, void \*, [**s64**](types_8h.md#typedef-s64), [**s64**](types_8h.md#typedef-s64)) <br> |
|  void | [**Finalize**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-finalize) () <br> |
|  [**Handle**](classnn_1_1_handle.md) | [**GetFileHandle**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-getfilehandle) (void \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**Initialize**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-initialize) ([**Handle**](classnn_1_1_handle.md) handle) <br> |
|  void \*\* | [**OpenDirect**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-opendirect-12) ([**Handle**](classnn_1_1_handle.md) handle) <br> |
|  void | [**OpenDirect**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-opendirect-22) (void \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryCreateDirectory**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-trycreatedirectory) (const wchar\_t \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryCreateDirectoryRaw**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-trycreatedirectoryraw) ([**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryCreateFile**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-trycreatefile) (const wchar\_t \*, [**s64**](types_8h.md#typedef-s64)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryDeleteDirectory**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-trydeletedirectory) (const wchar\_t \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryDeleteDirectoryRaw**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-trydeletedirectoryraw) ([**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryDeleteDirectoryRecursively**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-trydeletedirectoryrecursively) (const wchar\_t \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryDeleteDirectoryRecursivelyRaw**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-trydeletedirectoryrecursivelyraw) ([**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryDeleteFile**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-trydeletefile) (const wchar\_t \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryDeleteFileRaw**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-trydeletefileraw) ([**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryFlush**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-tryflush) (void \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryGetFileSize**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-trygetfilesize) ([**s64**](types_8h.md#typedef-s64) \*, const void \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryOpenDirectory**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-tryopendirectory) (void \*\*, const wchar\_t \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryOpenDirectoryRaw**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-tryopendirectoryraw) (void \*\*, [**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryOpenFile**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-tryopenfile) (void \*\*, const wchar\_t \*, [**bit32**](types_8h.md#typedef-bit32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryOpenFileRaw**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-tryopenfileraw) (void \*\*, [**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &, [**bit32**](types_8h.md#typedef-bit32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryOpenFileRawDirectly**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-tryopenfilerawdirectly) (void \*\*, [**bit32**](types_8h.md#typedef-bit32), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &, const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &, [**bit32**](types_8h.md#typedef-bit32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryReadDirectory**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-tryreaddirectory) ([**s32**](types_8h.md#typedef-s32) \*, void \*, class [**DirectoryEntry**](structnn_1_1fs_1_1_directory_entry.md) \*, [**s32**](types_8h.md#typedef-s32)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryReadFile**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-tryreadfile) ([**s32**](types_8h.md#typedef-s32) \*, void \*, [**s64**](types_8h.md#typedef-s64), void \*, size\_t) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryRenameDirectory**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-tryrenamedirectory) (const wchar\_t \*, const wchar\_t \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryRenameDirectoryRaw**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-tryrenamedirectoryraw) ([**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &, [**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryRenameFile**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-tryrenamefile) (const wchar\_t \*, const wchar\_t \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryRenameFileRaw**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-tryrenamefileraw) ([**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &, [**ArchiveHandle**](namespacenn_1_1fs.md#typedef-archivehandle), const [**Path**](namespacenn_1_1fs_1_1_c_t_r_1_1_m_p_core.md#typedef-path) &) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TrySetFileSize**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-trysetfilesize) (void \*, [**s64**](types_8h.md#typedef-s64)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryWriteFile**](classnn_1_1fs_1_1_c_t_r_1_1_m_p_core_1_1detail_1_1_user_file_system.md#function-trywritefile) ([**s32**](types_8h.md#typedef-s32) \*, void \*, [**s64**](types_8h.md#typedef-s64), const void \*, size\_t, bool) <br> |



















































------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fs/fs_FileSystemBase.h`

