

# Class nn::Handle



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**Handle**](classnn_1_1_handle.md)





* `#include <Handle.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**bit32**](types_8h.md#typedef-bit32) | [**GetPrintableBits**](#function-getprintablebits) () const<br> |
|   | [**Handle**](#function-handle-13) () <br> |
|   | [**Handle**](#function-handle-23) ([**nnHandle**](structnn_handle.md) handle) <br> |
|   | [**Handle**](#function-handle-33) ([**bit32**](types_8h.md#typedef-bit32) value) <br> |
|  bool | [**IsValid**](#function-isvalid) () const<br> |
|   | [**operator nnHandle**](#function-operator-nnhandle) () const<br> |
|  bool | [**operator!=**](#function-operator) (const [**Handle**](classnn_1_1_handle.md) & rhs) const<br> |
|  bool | [**operator==**](#function-operator_1) (const [**Handle**](classnn_1_1_handle.md) & rhs) const<br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**bit32**](types_8h.md#typedef-bit32) | [**m\_Handle**](#variable-m_handle)  <br> |




















## Public Functions Documentation




### function GetPrintableBits 

```C++
inline bit32 nn::Handle::GetPrintableBits () const
```




<hr>



### function Handle [1/3]

```C++
inline nn::Handle::Handle () 
```




<hr>



### function Handle [2/3]

```C++
inline nn::Handle::Handle (
    nnHandle handle
) 
```




<hr>



### function Handle [3/3]

```C++
inline nn::Handle::Handle (
    bit32 value
) 
```




<hr>



### function IsValid 

```C++
inline bool nn::Handle::IsValid () const
```




<hr>



### function operator nnHandle 

```C++
inline nn::Handle::operator nnHandle () const
```




<hr>



### function operator!= 

```C++
inline bool nn::Handle::operator!= (
    const Handle & rhs
) const
```




<hr>



### function operator== 

```C++
inline bool nn::Handle::operator== (
    const Handle & rhs
) const
```




<hr>
## Protected Attributes Documentation




### variable m\_Handle 

```C++
bit32 nn::Handle::m_Handle;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/Handle.h`

