

# File rvct\_stdio.cpp



[**FileList**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**rtport**](dir_53d6a9bf16b96d25f9c91e79a4c5362a.md) **>** [**rvct**](dir_00ebb32c10ea47286a1d484d586cc083.md) **>** [**rvct\_stdio.cpp**](rvct__stdio_8cpp.md)

[Go to the source code of this file](rvct__stdio_8cpp_source.md)



* `#include <cstring>`
* `#include <nn/assert.h>`
* `#include <nn/os/CTR/os_ThreadLocalRegion.h>`
* `#include <rt_misc.h>`
* `#include <rt_sys.h>`
* `#include <typeinfo>`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**std**](namespacestd.md) <br> |








## Public Attributes

| Type | Name |
| ---: | :--- |
|  const char | [**\_\_stderr\_name**](#variable-__stderr_name)   = `""`<br> |
|  const char | [**\_\_stdin\_name**](#variable-__stdin_name)   = `""`<br> |
|  const char | [**\_\_stdout\_name**](#variable-__stdout_name)   = `""`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**\_\_aeabi\_atexit**](#function-__aeabi_atexit) (void \* object, void(\*)(void \*) destructor, void \* dso\_handle) <br> |
|  void | [**\_\_rt\_div0**](#function-__rt_div0) () <br> |
|  void \*\* | [**\_\_rt\_eh\_globals\_addr**](#function-__rt_eh_globals_addr) () <br> |
|  void | [**\_\_rt\_raise**](#function-__rt_raise) (int sig, int type) <br> |
|  int | [**\_sys\_close**](#function-_sys_close) (FILEHANDLE fh) <br> |
|  long | [**\_sys\_flen**](#function-_sys_flen) (FILEHANDLE fh) <br> |
|  int | [**\_sys\_istty**](#function-_sys_istty) (FILEHANDLE fh) <br> |
|  FILEHANDLE | [**\_sys\_open**](#function-_sys_open) (const char \* name, int openmode) <br> |
|  int | [**\_sys\_read**](#function-_sys_read) (FILEHANDLE fh, unsigned char \* buf, unsigned int len, int mode) <br> |
|  int | [**\_sys\_seek**](#function-_sys_seek) (FILEHANDLE fh, long pos) <br> |
|  int | [**\_sys\_write**](#function-_sys_write) (FILEHANDLE fh, const unsigned char \* buf, unsigned int len, int mode) <br> |
|  void | [**abort**](#function-abort) () <br> |




























## Public Attributes Documentation




### variable \_\_stderr\_name 

```C++
const char __stderr_name[];
```




<hr>



### variable \_\_stdin\_name 

```C++
const char __stdin_name[];
```




<hr>



### variable \_\_stdout\_name 

```C++
const char __stdout_name[];
```




<hr>
## Public Functions Documentation




### function \_\_aeabi\_atexit 

```C++
void __aeabi_atexit (
    void * object,
    void(*)(void *) destructor,
    void * dso_handle
) 
```




<hr>



### function \_\_rt\_div0 

```C++
void __rt_div0 () 
```




<hr>



### function \_\_rt\_eh\_globals\_addr 

```C++
void ** __rt_eh_globals_addr () 
```




<hr>



### function \_\_rt\_raise 

```C++
void __rt_raise (
    int sig,
    int type
) 
```




<hr>



### function \_sys\_close 

```C++
int _sys_close (
    FILEHANDLE fh
) 
```




<hr>



### function \_sys\_flen 

```C++
long _sys_flen (
    FILEHANDLE fh
) 
```




<hr>



### function \_sys\_istty 

```C++
int _sys_istty (
    FILEHANDLE fh
) 
```




<hr>



### function \_sys\_open 

```C++
FILEHANDLE _sys_open (
    const char * name,
    int openmode
) 
```




<hr>



### function \_sys\_read 

```C++
int _sys_read (
    FILEHANDLE fh,
    unsigned char * buf,
    unsigned int len,
    int mode
) 
```




<hr>



### function \_sys\_seek 

```C++
int _sys_seek (
    FILEHANDLE fh,
    long pos
) 
```




<hr>



### function \_sys\_write 

```C++
int _sys_write (
    FILEHANDLE fh,
    const unsigned char * buf,
    unsigned int len,
    int mode
) 
```




<hr>



### function abort 

```C++
void abort () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/sources/libraries/rtport/rvct/rvct_stdio.cpp`

