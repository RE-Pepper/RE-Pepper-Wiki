

# File os\_CppException.cpp



[**FileList**](files.md) **>** [**CTR**](dir_9d5035ea42e3a15a3c12a88837862b5a.md) **>** [**os\_CppException.cpp**](os___cpp_exception_8cpp.md)

[Go to the source code of this file](os___cpp_exception_8cpp_source.md)



* `#include <cstdlib>`
* `#include <exception>`
* `#include <nn/os/CTR/os_CppException.h>`
* `#include <nn/os/CTR/os_ThreadLocalRegion.h>`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**nn**](namespacenn.md) <br> |
| namespace | [**os**](namespacenn_1_1os.md) <br> |
| namespace | [**CTR**](namespacenn_1_1os_1_1_c_t_r.md) <br> |








## Public Attributes

| Type | Name |
| ---: | :--- |
|  handler | [**call\_hook**](#variable-call_hook)  <br> |
|  void \* | [**caughtExceptions**](#variable-caughtexceptions)  <br> |
|  void \* | [**emergency\_buffer**](#variable-emergency_buffer)  <br> |
|  bool | [**implementation\_ever\_called\_terminate**](#variable-implementation_ever_called_terminate)  <br> |
|  void \* | [**propagatingExceptions**](#variable-propagatingexceptions)  <br> |
|  std::terminate\_handler | [**terminateHandler**](#variable-terminatehandler)  <br> |
|  uint32\_t | [**uncaughtExceptions**](#variable-uncaughtexceptions)  <br> |
|  std::unexpected\_handler | [**unexpectedHandler**](#variable-unexpectedhandler)  <br> |












































## Public Attributes Documentation




### variable call\_hook 

```C++
handler call_hook;
```




<hr>



### variable caughtExceptions 

```C++
void* caughtExceptions;
```




<hr>



### variable emergency\_buffer 

```C++
void* emergency_buffer;
```




<hr>



### variable implementation\_ever\_called\_terminate 

```C++
bool implementation_ever_called_terminate;
```




<hr>



### variable propagatingExceptions 

```C++
void* propagatingExceptions;
```




<hr>



### variable terminateHandler 

```C++
std::terminate_handler terminateHandler;
```




<hr>



### variable uncaughtExceptions 

```C++
uint32_t uncaughtExceptions;
```




<hr>



### variable unexpectedHandler 

```C++
std::unexpected_handler unexpectedHandler;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/sources/libraries/os/CTR/os_CppException.cpp`

