

# Struct nn::os::CTR::ThreadLocalRegion



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**os**](namespacenn_1_1os.md) **>** [**CTR**](namespacenn_1_1os_1_1_c_t_r.md) **>** [**ThreadLocalRegion**](structnn_1_1os_1_1_c_t_r_1_1_thread_local_region.md)





* `#include <os_ThreadLocalRegion.h>`





















## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**bit32**](types_8h.md#typedef-bit32) | [**ehGlobals**](#variable-ehglobals)  <br> |
|  void \* | [**ehGlobalsAddr**](#variable-ehglobalsaddr)  <br> |
|  [**uptr**](types_8h.md#typedef-uptr) | [**handlerAddress**](#variable-handleraddress)  <br> |
|  [**uptr**](types_8h.md#typedef-uptr) | [**handlerStackBottomAddress**](#variable-handlerstackbottomaddress)  <br> |
|  [**bit32**](types_8h.md#typedef-bit32) | [**messageBuffer**](#variable-messagebuffer)  <br> |
|  [**bit32**](types_8h.md#typedef-bit32) | [**receiveBuffer**](#variable-receivebuffer)  <br> |
|  [**bit8**](types_8h.md#typedef-bit8) | [**reserved**](#variable-reserved)  <br> |
|  [**uptr**](types_8h.md#typedef-uptr) | [**tls**](#variable-tls)  <br> |












































## Public Attributes Documentation




### variable ehGlobals 

```C++
bit32 nn::os::CTR::ThreadLocalRegion::ehGlobals[8];
```




<hr>



### variable ehGlobalsAddr 

```C++
void* nn::os::CTR::ThreadLocalRegion::ehGlobalsAddr;
```




<hr>



### variable handlerAddress 

```C++
uptr nn::os::CTR::ThreadLocalRegion::handlerAddress;
```




<hr>



### variable handlerStackBottomAddress 

```C++
uptr nn::os::CTR::ThreadLocalRegion::handlerStackBottomAddress;
```




<hr>



### variable messageBuffer 

```C++
bit32 nn::os::CTR::ThreadLocalRegion::messageBuffer[64];
```




<hr>



### variable receiveBuffer 

```C++
bit32 nn::os::CTR::ThreadLocalRegion::receiveBuffer[32];
```




<hr>



### variable reserved 

```C++
bit8 nn::os::CTR::ThreadLocalRegion::reserved[20];
```




<hr>



### variable tls 

```C++
uptr nn::os::CTR::ThreadLocalRegion::tls[16];
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/os/CTR/os_ThreadLocalRegion.h`

