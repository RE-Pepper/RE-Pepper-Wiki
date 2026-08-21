

# Class nn::fs::detail::FileBaseImpl



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fs**](namespacenn_1_1fs.md) **>** [**detail**](namespacenn_1_1fs_1_1detail.md) **>** [**FileBaseImpl**](classnn_1_1fs_1_1detail_1_1_file_base_impl.md)





* `#include <fs_FileBase.h>`



Inherits the following classes: [nn::util::ADLFireWall::NonCopyable](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**FileBaseImpl**](#function-filebaseimpl) () <br> |
|  void | [**Finalize**](#function-finalize) () <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryFlush**](#function-tryflush) () <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryGetSize**](#function-trygetsize) ([**s64**](types_8h.md#typedef-s64) \* pOut) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryOpenImpl**](#function-tryopenimpl) (const wchar\_t \* path, [**bit32**](types_8h.md#typedef-bit32) mode) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryRead**](#function-tryread) ([**s32**](types_8h.md#typedef-s32) \* pOut, [**s64**](types_8h.md#typedef-s64) offset, void \* buffer, size\_t size) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TrySetSize**](#function-trysetsize) ([**s64**](types_8h.md#typedef-s64) size) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryWrite**](#function-trywrite) ([**s32**](types_8h.md#typedef-s32) \* pOut, [**s64**](types_8h.md#typedef-s64) offset, const void \* buffer, size\_t size, bool flush) <br> |
|   | [**~FileBaseImpl**](#function-filebaseimpl) () <br> |


















































## Protected Functions inherited from nn::util::ADLFireWall::NonCopyable

See [nn::util::ADLFireWall::NonCopyable](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md)

| Type | Name |
| ---: | :--- |
|   | [**NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable-12) () <br> |
|   | [**~NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable) () <br> |






## Public Functions Documentation




### function FileBaseImpl 

```C++
inline nn::fs::detail::FileBaseImpl::FileBaseImpl () 
```




<hr>



### function Finalize 

```C++
inline void nn::fs::detail::FileBaseImpl::Finalize () 
```




<hr>



### function TryFlush 

```C++
inline Result nn::fs::detail::FileBaseImpl::TryFlush () 
```




<hr>



### function TryGetSize 

```C++
inline Result nn::fs::detail::FileBaseImpl::TryGetSize (
    s64 * pOut
) 
```




<hr>



### function TryOpenImpl 

```C++
inline Result nn::fs::detail::FileBaseImpl::TryOpenImpl (
    const wchar_t * path,
    bit32 mode
) 
```




<hr>



### function TryRead 

```C++
inline Result nn::fs::detail::FileBaseImpl::TryRead (
    s32 * pOut,
    s64 offset,
    void * buffer,
    size_t size
) 
```




<hr>



### function TrySetSize 

```C++
inline Result nn::fs::detail::FileBaseImpl::TrySetSize (
    s64 size
) 
```




<hr>



### function TryWrite 

```C++
inline Result nn::fs::detail::FileBaseImpl::TryWrite (
    s32 * pOut,
    s64 offset,
    const void * buffer,
    size_t size,
    bool flush
) 
```




<hr>



### function ~FileBaseImpl 

```C++
inline nn::fs::detail::FileBaseImpl::~FileBaseImpl () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fs/CTR/MPCore/fs_FileBase.h`

