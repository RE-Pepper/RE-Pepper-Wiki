

# Class nn::os::Thread



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**os**](namespacenn_1_1os.md) **>** [**Thread**](classnn_1_1os_1_1_thread.md)





* `#include <os_Thread.h>`



Inherits the following classes: [nn::os::WaitObject](classnn_1_1os_1_1_wait_object.md)






























































































## Public Functions

| Type | Name |
| ---: | :--- |
|  void \* | [**CallDestructorAndExit**](#function-calldestructorandexit) () <br> |
|  void | [**ChangeCurrentPriority**](#function-changecurrentpriority) ([**s32**](types_8h.md#typedef-s32) priority) <br> |
|  void | [**ChangePriority**](#function-changepriority) ([**s32**](types_8h.md#typedef-s32) priority) <br> |
|  void | [**Finalize**](#function-finalize) () <br> |
|  void | [**FinalizeImpl**](#function-finalizeimpl) () <br> |
|  [**bit32**](types_8h.md#typedef-bit32) | [**GetCurrentId**](#function-getcurrentid) () const<br> |
|  [**s32**](types_8h.md#typedef-s32) | [**GetCurrentPriority**](#function-getcurrentpriority) () const<br> |
|  [**s32**](types_8h.md#typedef-s32) | [**GetCurrentProcessorNumber**](#function-getcurrentprocessornumber) () const<br> |
|  [**s32**](types_8h.md#typedef-s32) | [**GetDefaultIdealProcessor**](#function-getdefaultidealprocessor) () const<br> |
|  [**bit32**](types_8h.md#typedef-bit32) | [**GetId**](#function-getid) () const<br> |
|  [**s32**](types_8h.md#typedef-s32) | [**GetIdealProcessor**](#function-getidealprocessor) () const<br> |
|  [**s32**](types_8h.md#typedef-s32) | [**GetPriority**](#function-getpriority) () const<br> |
|  bool | [**IsAlive**](#function-isalive) () const<br> |
|  void | [**Join**](#function-join) () <br> |
|  void | [**NoParameterFunc**](#function-noparameterfunc) (void(\*)() f) <br> |
|  void | [**SetAutoStackManager**](#function-setautostackmanager) ([**AutoStackManager**](classnn_1_1os_1_1_thread.md#typedef-autostackmanager) \* pManager) <br> |
|  void | [**Sleep**](#function-sleep) ([**fnd::TimeSpan**](classnn_1_1fnd_1_1_time_span.md) span) <br> |
|  void | [**SleepImpl**](#function-sleepimpl) ([**fnd::TimeSpan**](classnn_1_1fnd_1_1_time_span.md) span) <br> |
|  void | [**Start**](#function-start) (void(\*)(T1) f, T2 param, Stack & stack, [**s32**](types_8h.md#typedef-s32) priority, [**s32**](types_8h.md#typedef-s32) coreNo=254) <br> |
|  void | [**StartUsingAutoStack**](#function-startusingautostack) (T1 f, T2 param, size\_t stackSize, [**s32**](types_8h.md#typedef-s32) priority, [**s32**](types_8h.md#typedef-s32) coreNo) <br> |
|   | [**Thread**](#function-thread-12) () <br> |
|   | [**Thread**](#function-thread-22) (const [**InitializeAsCurrentTag**](structnn_1_1os_1_1_thread_1_1_initialize_as_current_tag.md) &) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryInitializeAndStartImpl**](#function-tryinitializeandstartimpl) ([**TypeInfo**](structnn_1_1os_1_1_thread_1_1_type_info.md) typeInfo, [**ThreadFunc**](namespacenn_1_1os.md#typedef-threadfunc) f, const void \* p, [**uptr**](types_8h.md#typedef-uptr) stackBottom, [**s32**](types_8h.md#typedef-s32) priority, [**s32**](types_8h.md#typedef-s32) coreNo, bool isAutoStack) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryInitializeAndStartImplUsingAutoStack**](#function-tryinitializeandstartimplusingautostack) ([**TypeInfo**](structnn_1_1os_1_1_thread_1_1_type_info.md) typeInfo, [**ThreadFunc**](namespacenn_1_1os.md#typedef-threadfunc) f, const void \* p, size\_t stackSize, [**s32**](types_8h.md#typedef-s32) priority, [**s32**](types_8h.md#typedef-s32) coreNo) <br> |
|  [**Result**](classnn_1_1_result.md) | [**TryStart**](#function-trystart) (void(\*)(T1) f, T2 param, Stack \* stack, [**s32**](types_8h.md#typedef-s32) priority, [**s32**](types_8h.md#typedef-s32) coreNo) <br> |
|  void | [**Yield**](#function-yield) () <br> |
|   | [**~Thread**](#function-thread) () <br> |


## Public Functions inherited from nn::os::WaitObject

See [nn::os::WaitObject](classnn_1_1os_1_1_wait_object.md)

| Type | Name |
| ---: | :--- |
|   | [**WaitObject**](classnn_1_1os_1_1_wait_object.md#function-waitobject) () <br> |
|  void | [**WaitOne**](classnn_1_1os_1_1_wait_object.md#function-waitone-12) () <br> |
|  bool | [**WaitOne**](classnn_1_1os_1_1_wait_object.md#function-waitone-22) ([**fnd::TimeSpan**](classnn_1_1fnd_1_1_time_span.md) timeout) <br> |
|  [**Result**](classnn_1_1_result.md) | [**WaitOneImpl**](classnn_1_1os_1_1_wait_object.md#function-waitoneimpl) ([**s64**](types_8h.md#typedef-s64) nanoSecondsTimeout) <br> |
|   | [**~WaitObject**](classnn_1_1os_1_1_wait_object.md#function-waitobject) () <br> |


## Public Functions inherited from nn::os::HandleObject

See [nn::os::HandleObject](classnn_1_1os_1_1_handle_object.md)

| Type | Name |
| ---: | :--- |
|  void | [**ClearHandle**](classnn_1_1os_1_1_handle_object.md#function-clearhandle) () <br> |
|  void | [**Close**](classnn_1_1os_1_1_handle_object.md#function-close) () <br> |
|  void | [**Finalize**](classnn_1_1os_1_1_handle_object.md#function-finalize) () <br> |
|   | [**HandleObject**](classnn_1_1os_1_1_handle_object.md#function-handleobject) () <br> |
|  void | [**SetHandle**](classnn_1_1os_1_1_handle_object.md#function-sethandle) ([**Handle**](classnn_1_1_handle.md) handle) <br> |
|   | [**~HandleObject**](classnn_1_1os_1_1_handle_object.md#function-handleobject) () <br> |




## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**Thread**](classnn_1_1os_1_1_thread.md) & | [**GetMainThread**](#function-getmainthread) () <br> |
|  void | [**OnThreadExit**](#function-onthreadexit) () <br> |
|  void | [**OnThreadStart**](#function-onthreadstart) () <br> |
|  void | [**ThreadStart**](#function-threadstart) ([**uptr**](types_8h.md#typedef-uptr) p) <br> |


## Public Static Functions inherited from nn::os::WaitObject

See [nn::os::WaitObject](classnn_1_1os_1_1_wait_object.md)

| Type | Name |
| ---: | :--- |
|  [**s32**](types_8h.md#typedef-s32) | [**WaitAny**](classnn_1_1os_1_1_wait_object.md#function-waitany) ([**WaitObject**](classnn_1_1os_1_1_wait_object.md) \*\* objs, [**s32**](types_8h.md#typedef-s32) numObjects) <br> |


























































































## Protected Functions inherited from nn::os::HandleObject

See [nn::os::HandleObject](classnn_1_1os_1_1_handle_object.md)

| Type | Name |
| ---: | :--- |
|  [**Handle**](classnn_1_1_handle.md) | [**GetHandle**](classnn_1_1os_1_1_handle_object.md#function-gethandle) () const<br> |
|  bool | [**IsValid**](classnn_1_1os_1_1_handle_object.md#function-isvalid) () const<br> |


## Protected Functions inherited from nn::util::ADLFireWall::NonCopyable

See [nn::util::ADLFireWall::NonCopyable](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md)

| Type | Name |
| ---: | :--- |
|   | [**NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable-12) () <br> |
|   | [**~NonCopyable**](structnn_1_1util_1_1_a_d_l_fire_wall_1_1_non_copyable.md#function-noncopyable) () <br> |










## Public Functions Documentation




### function CallDestructorAndExit 

```C++
void * nn::os::Thread::CallDestructorAndExit () 
```




<hr>



### function ChangeCurrentPriority 

```C++
inline void nn::os::Thread::ChangeCurrentPriority (
    s32 priority
) 
```




<hr>



### function ChangePriority 

```C++
inline void nn::os::Thread::ChangePriority (
    s32 priority
) 
```




<hr>



### function Finalize 

```C++
inline void nn::os::Thread::Finalize () 
```




<hr>



### function FinalizeImpl 

```C++
void nn::os::Thread::FinalizeImpl () 
```




<hr>



### function GetCurrentId 

```C++
inline bit32 nn::os::Thread::GetCurrentId () const
```




<hr>



### function GetCurrentPriority 

```C++
inline s32 nn::os::Thread::GetCurrentPriority () const
```




<hr>



### function GetCurrentProcessorNumber 

```C++
inline s32 nn::os::Thread::GetCurrentProcessorNumber () const
```




<hr>



### function GetDefaultIdealProcessor 

```C++
inline s32 nn::os::Thread::GetDefaultIdealProcessor () const
```




<hr>



### function GetId 

```C++
inline bit32 nn::os::Thread::GetId () const
```




<hr>



### function GetIdealProcessor 

```C++
inline s32 nn::os::Thread::GetIdealProcessor () const
```




<hr>



### function GetPriority 

```C++
inline s32 nn::os::Thread::GetPriority () const
```




<hr>



### function IsAlive 

```C++
inline bool nn::os::Thread::IsAlive () const
```




<hr>



### function Join 

```C++
void nn::os::Thread::Join () 
```




<hr>



### function NoParameterFunc 

```C++
void nn::os::Thread::NoParameterFunc (
    void(*)() f
) 
```




<hr>



### function SetAutoStackManager 

```C++
inline void nn::os::Thread::SetAutoStackManager (
    AutoStackManager * pManager
) 
```




<hr>



### function Sleep 

```C++
inline void nn::os::Thread::Sleep (
    fnd::TimeSpan span
) 
```




<hr>



### function SleepImpl 

```C++
void nn::os::Thread::SleepImpl (
    fnd::TimeSpan span
) 
```




<hr>



### function Start 

```C++
template<typename T1, typename T2, typename Stack>
inline void nn::os::Thread::Start (
    void(*)(T1) f,
    T2 param,
    Stack & stack,
    s32 priority,
    s32 coreNo=254
) 
```




<hr>



### function StartUsingAutoStack 

```C++
template<typename T1, typename T2, typename Thread>
inline void nn::os::Thread::StartUsingAutoStack (
    T1 f,
    T2 param,
    size_t stackSize,
    s32 priority,
    s32 coreNo
) 
```




<hr>



### function Thread [1/2]

```C++
inline nn::os::Thread::Thread () 
```




<hr>



### function Thread [2/2]

```C++
nn::os::Thread::Thread (
    const InitializeAsCurrentTag &
) 
```




<hr>



### function TryInitializeAndStartImpl 

```C++
Result nn::os::Thread::TryInitializeAndStartImpl (
    TypeInfo typeInfo,
    ThreadFunc f,
    const void * p,
    uptr stackBottom,
    s32 priority,
    s32 coreNo,
    bool isAutoStack
) 
```




<hr>



### function TryInitializeAndStartImplUsingAutoStack 

```C++
Result nn::os::Thread::TryInitializeAndStartImplUsingAutoStack (
    TypeInfo typeInfo,
    ThreadFunc f,
    const void * p,
    size_t stackSize,
    s32 priority,
    s32 coreNo
) 
```




<hr>



### function TryStart 

```C++
template<typename T1, typename T2, typename Stack>
inline Result nn::os::Thread::TryStart (
    void(*)(T1) f,
    T2 param,
    Stack * stack,
    s32 priority,
    s32 coreNo
) 
```




<hr>



### function Yield 

```C++
inline void nn::os::Thread::Yield () 
```




<hr>



### function ~Thread 

```C++
inline nn::os::Thread::~Thread () 
```




<hr>
## Public Static Functions Documentation




### function GetMainThread 

```C++
static inline Thread & nn::os::Thread::GetMainThread () 
```




<hr>



### function OnThreadExit 

```C++
static void nn::os::Thread::OnThreadExit () 
```




<hr>



### function OnThreadStart 

```C++
static void nn::os::Thread::OnThreadStart () 
```




<hr>



### function ThreadStart 

```C++
static void nn::os::Thread::ThreadStart (
    uptr p
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/os/os_Thread.h`

