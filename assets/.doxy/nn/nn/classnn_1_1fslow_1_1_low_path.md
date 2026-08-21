

# Class nn::fslow::LowPath

**template &lt;class T, typename V&gt;**



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fslow**](namespacenn_1_1fslow.md) **>** [**LowPath**](classnn_1_1fslow_1_1_low_path.md)





* `#include <fslow_Path.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|  const void \* | [**GetDataBuffer**](#function-getdatabuffer) () <br> |
|  size\_t | [**GetDataSize**](#function-getdatasize) () <br> |
|  [**bit32**](types_8h.md#typedef-bit32) | [**GetPathType**](#function-getpathtype) () <br> |
|  const wchar\_t \* | [**GetWStringRaw**](#function-getwstringraw) () <br> |
|   | [**LowPath**](#function-lowpath-12) () <br> |
|   | [**LowPath**](#function-lowpath-22) (const wchar\_t \* path) <br> |
|  void | [**SetBinary**](#function-setbinary) (const T \* p) <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**LowPath**](classnn_1_1fslow_1_1_low_path.md) | [**Make**](#function-make) (const T \* p) <br> |


























## Public Functions Documentation




### function GetDataBuffer 

```C++
inline const void * nn::fslow::LowPath::GetDataBuffer () 
```




<hr>



### function GetDataSize 

```C++
inline size_t nn::fslow::LowPath::GetDataSize () 
```




<hr>



### function GetPathType 

```C++
inline bit32 nn::fslow::LowPath::GetPathType () 
```




<hr>



### function GetWStringRaw 

```C++
inline const wchar_t * nn::fslow::LowPath::GetWStringRaw () 
```




<hr>



### function LowPath [1/2]

```C++
inline nn::fslow::LowPath::LowPath () 
```




<hr>



### function LowPath [2/2]

```C++
inline nn::fslow::LowPath::LowPath (
    const wchar_t * path
) 
```




<hr>



### function SetBinary 

```C++
inline void nn::fslow::LowPath::SetBinary (
    const T * p
) 
```




<hr>
## Public Static Functions Documentation




### function Make 

```C++
static inline LowPath nn::fslow::LowPath::Make (
    const T * p
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fslow/fslow_Path.h`

