

# Class nn::fs::detail::FileSystemBase



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fs**](namespacenn_1_1fs.md) **>** [**detail**](namespacenn_1_1fs_1_1detail.md) **>** [**FileSystemBase**](classnn_1_1fs_1_1detail_1_1_file_system_base.md)





* `#include <fs_FileSystemBase.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**FileSystemBase**](#function-filesystembase-13) () <br> |
|   | [**FileSystemBase**](#function-filesystembase-23) (int \* a) <br> |
|   | [**FileSystemBase**](#function-filesystembase-13) () <br> |
|  void | [**Initialize**](#function-initialize) ([**FileSystemBaseImpl**](classnn_1_1fs_1_1detail_1_1_file_system_base_impl.md) \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryCreateDirectory**](#function-trycreatedirectory) (const char \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryCreateFile**](#function-trycreatefile) (const char \*, [**s64**](types_8h.md#typedef-s64)) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryDeleteFile**](#function-trydeletefile) (const char \*) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryRenameFile**](#function-tryrenamefile) (const char \*, const char \*) <br> |




























## Public Functions Documentation




### function FileSystemBase [1/3]

```C++
inline nn::fs::detail::FileSystemBase::FileSystemBase () 
```




<hr>



### function FileSystemBase [2/3]

```C++
inline nn::fs::detail::FileSystemBase::FileSystemBase (
    int * a
) 
```




<hr>



### function FileSystemBase [1/3]

```C++
nn::fs::detail::FileSystemBase::FileSystemBase () 
```




<hr>



### function Initialize 

```C++
void nn::fs::detail::FileSystemBase::Initialize (
    FileSystemBaseImpl *
) 
```




<hr>



### function TryCreateDirectory 

```C++
Result nn::fs::detail::FileSystemBase::TryCreateDirectory (
    const char *
) 
```




<hr>



### function TryCreateFile 

```C++
Result nn::fs::detail::FileSystemBase::TryCreateFile (
    const char *,
    s64
) 
```




<hr>



### function TryDeleteFile 

```C++
Result nn::fs::detail::FileSystemBase::TryDeleteFile (
    const char *
) 
```




<hr>



### function TryRenameFile 

```C++
Result nn::fs::detail::FileSystemBase::TryRenameFile (
    const char *,
    const char *
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fs/detail/fs_FileSystemBase.h`

