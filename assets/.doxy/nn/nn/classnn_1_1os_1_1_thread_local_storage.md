

# Class nn::os::ThreadLocalStorage



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**os**](namespacenn_1_1os.md) **>** [**ThreadLocalStorage**](classnn_1_1os_1_1_thread_local_storage.md)





* `#include <os_ThreadLocalStorage.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**uptr**](types_8h.md#typedef-uptr) | [**GetValue**](#function-getvalue) () const<br> |
|  void | [**SetValue**](#function-setvalue) ([**uptr**](types_8h.md#typedef-uptr) value) <br> |
|   | [**ThreadLocalStorage**](#function-threadlocalstorage) () <br> |
|   | [**~ThreadLocalStorage**](#function-threadlocalstorage) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**ClearAllSlots**](#function-clearallslots) () <br> |


























## Public Functions Documentation




### function GetValue 

```C++
uptr nn::os::ThreadLocalStorage::GetValue () const
```




<hr>



### function SetValue 

```C++
void nn::os::ThreadLocalStorage::SetValue (
    uptr value
) 
```




<hr>



### function ThreadLocalStorage 

```C++
nn::os::ThreadLocalStorage::ThreadLocalStorage () 
```




<hr>



### function ~ThreadLocalStorage 

```C++
nn::os::ThreadLocalStorage::~ThreadLocalStorage () 
```




<hr>
## Public Static Functions Documentation




### function ClearAllSlots 

```C++
static void nn::os::ThreadLocalStorage::ClearAllSlots () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/os/os_ThreadLocalStorage.h`

