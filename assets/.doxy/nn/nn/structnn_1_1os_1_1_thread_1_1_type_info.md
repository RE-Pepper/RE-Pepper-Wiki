

# Struct nn::os::Thread::TypeInfo



[**ClassList**](annotated.md) **>** [**TypeInfo**](structnn_1_1os_1_1_thread_1_1_type_info.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  void(\* | [**copy**](#variable-copy)  <br> |
|  void(\* | [**destroy**](#variable-destroy)  <br> |
|  void(\* | [**invoke**](#variable-invoke)  <br> |
|  size\_t | [**size**](#variable-size)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**Copy**](#function-copy) (const void \* src, void \* dst) <br> |
|  void | [**Destroy**](#function-destroy) (void \* p) <br> |
|  void | [**Invoke**](#function-invoke) ([**ThreadFunc**](namespacenn_1_1os.md#typedef-threadfunc) f, const void \* p) <br> |
|  void | [**SetData**](#function-setdata) () <br> |




























## Public Attributes Documentation




### variable copy 

```C++
void(* nn::os::Thread::TypeInfo::copy) (const void *src, void *dsr);
```




<hr>



### variable destroy 

```C++
void(* nn::os::Thread::TypeInfo::destroy) (void *p);
```




<hr>



### variable invoke 

```C++
void(* nn::os::Thread::TypeInfo::invoke) (ThreadFunc f, const void *p);
```




<hr>



### variable size 

```C++
size_t nn::os::Thread::TypeInfo::size;
```




<hr>
## Public Functions Documentation




### function Copy 

```C++
template<typename T1, typename T2>
inline void TypeInfo::Copy (
    const void * src,
    void * dst
) 
```




<hr>



### function Destroy 

```C++
template<typename T>
inline void TypeInfo::Destroy (
    void * p
) 
```




<hr>



### function Invoke 

```C++
template<typename T>
inline void TypeInfo::Invoke (
    ThreadFunc f,
    const void * p
) 
```




<hr>



### function SetData 

```C++
template<typename T1, typename T2, typename T3>
inline void TypeInfo::SetData () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/os/os_Thread.h`

