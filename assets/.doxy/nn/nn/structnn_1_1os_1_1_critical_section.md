

# Struct nn::os::CriticalSection



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**os**](namespacenn_1_1os.md) **>** [**CriticalSection**](structnn_1_1os_1_1_critical_section.md)





* `#include <os_CriticalSection.h>`



Inherits the following classes: [nn::util::ADLFireWall::NonCopyable](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md)












## Classes

| Type | Name |
| ---: | :--- |
| struct | [**ScopedLock**](structnn_1_1os_1_1_critical_section_1_1_scoped_lock.md) <br> |










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**CriticalSection**](#function-criticalsection-12) () <br> |
|   | [**CriticalSection**](#function-criticalsection-22) (const [**WithInitialize**](classnn_1_1_with_initialize.md) &) <br> |
|  void | [**Enter**](#function-enter) () <br> |
|  void | [**EnterImpl**](#function-enterimpl) () <br> |
|  void | [**Finalize**](#function-finalize) () <br> |
|  [**uptr**](types_8h.md#typedef-uptr) | [**GetInvalidThreadUniqueValue**](#function-getinvalidthreaduniquevalue) () <br> |
|  [**uptr**](types_8h.md#typedef-uptr) | [**GetThreadUniqueValue**](#function-getthreaduniquevalue) () <br> |
|  void | [**Initialize**](#function-initialize) () <br> |
|  bool | [**IsInitialized**](#function-isinitialized) () const<br> |
|  void | [**Leave**](#function-leave) () <br> |
|  bool | [**LockedByCurrentThread**](#function-lockedbycurrentthread) () <br> |
|  bool | [**TryEnter**](#function-tryenter) () <br> |
|  bool | [**TryEnterImpl**](#function-tryenterimpl) () <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryInitialize**](#function-tryinitialize) () <br> |
|   | [**~CriticalSection**](#function-criticalsection) () <br> |


















































## Protected Functions inherited from nn::util::ADLFireWall::NonCopyable

See [nn::util::ADLFireWall::NonCopyable](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md)

| Type | Name |
| ---: | :--- |
|   | [**NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable-12) () <br> |
|   | [**~NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable) () <br> |






## Public Functions Documentation




### function CriticalSection [1/2]

```C++
inline nn::os::CriticalSection::CriticalSection () 
```




<hr>



### function CriticalSection [2/2]

```C++
inline nn::os::CriticalSection::CriticalSection (
    const WithInitialize &
) 
```




<hr>



### function Enter 

```C++
inline void nn::os::CriticalSection::Enter () 
```




<hr>



### function EnterImpl 

```C++
void nn::os::CriticalSection::EnterImpl () 
```




<hr>



### function Finalize 

```C++
inline void nn::os::CriticalSection::Finalize () 
```




<hr>



### function GetInvalidThreadUniqueValue 

```C++
inline uptr nn::os::CriticalSection::GetInvalidThreadUniqueValue () 
```




<hr>



### function GetThreadUniqueValue 

```C++
inline uptr nn::os::CriticalSection::GetThreadUniqueValue () 
```




<hr>



### function Initialize 

```C++
inline void nn::os::CriticalSection::Initialize () 
```




<hr>



### function IsInitialized 

```C++
inline bool nn::os::CriticalSection::IsInitialized () const
```




<hr>



### function Leave 

```C++
inline void nn::os::CriticalSection::Leave () 
```




<hr>



### function LockedByCurrentThread 

```C++
inline bool nn::os::CriticalSection::LockedByCurrentThread () 
```




<hr>



### function TryEnter 

```C++
inline bool nn::os::CriticalSection::TryEnter () 
```




<hr>



### function TryEnterImpl 

```C++
inline bool nn::os::CriticalSection::TryEnterImpl () 
```




<hr>



### function TryInitialize 

```C++
inline Result nn::os::CriticalSection::TryInitialize () 
```




<hr>



### function ~CriticalSection 

```C++
inline nn::os::CriticalSection::~CriticalSection () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/os/os_CriticalSection.h`

