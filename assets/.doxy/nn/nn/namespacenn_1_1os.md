

# Namespace nn::os



[**Namespace List**](namespaces.md) **>** [**nn**](namespacenn.md) **>** [**os**](namespacenn_1_1os.md)


















## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**CTR**](namespacenn_1_1os_1_1_c_t_r.md) <br> |
| namespace | [**detail**](namespacenn_1_1os_1_1detail.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| struct | [**CriticalSection**](structnn_1_1os_1_1_critical_section.md) <br> |
| class | [**Event**](classnn_1_1os_1_1_event.md) <br> |
| class | [**EventBase**](classnn_1_1os_1_1_event_base.md) <br> |
| class | [**FlagsEnum**](classnn_1_1os_1_1_flags_enum.md) &lt;typename T, typename V&gt;<br> |
| struct | [**FlagsEnum1**](structnn_1_1os_1_1_flags_enum1.md) &lt;typename V&gt;<br> |
| struct | [**FlagsEnum2**](structnn_1_1os_1_1_flags_enum2.md) &lt;typename V&gt;<br> |
| struct | [**FlagsEnum4**](structnn_1_1os_1_1_flags_enum4.md) &lt;typename V&gt;<br> |
| class | [**HandleObject**](classnn_1_1os_1_1_handle_object.md) <br> |
| class | [**InterruptEvent**](classnn_1_1os_1_1_interrupt_event.md) <br> |
| class | [**LightEvent**](classnn_1_1os_1_1_light_event.md) <br> |
| class | [**LightSemaphore**](classnn_1_1os_1_1_light_semaphore.md) <br> |
| struct | [**MemoryInfo**](structnn_1_1os_1_1_memory_info.md) <br> |
| struct | [**PageInfo**](structnn_1_1os_1_1_page_info.md) <br> |
| struct | [**ReadOnlySharedInfo**](structnn_1_1os_1_1_read_only_shared_info.md) <br> |
| struct | [**RtcSwcInfo**](structnn_1_1os_1_1_rtc_swc_info.md) <br> |
| struct | [**Semaphore**](structnn_1_1os_1_1_semaphore.md) <br> |
| class | [**StackBuffer**](classnn_1_1os_1_1_stack_buffer.md) &lt;Size&gt;<br> |
| class | [**Thread**](classnn_1_1os_1_1_thread.md) <br> |
| class | [**ThreadLocalStorage**](classnn_1_1os_1_1_thread_local_storage.md) <br> |
| class | [**Tick**](classnn_1_1os_1_1_tick.md) <br> |
| class | [**WaitObject**](classnn_1_1os_1_1_wait_object.md) <br> |
| class | [**WaitableCounter**](classnn_1_1os_1_1_waitable_counter.md) <br> |
| struct | [**WritableSharedInfo**](structnn_1_1os_1_1_writable_shared_info.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| enum  | [**ArbitrationType**](#enum-arbitrationtype)  <br> |
| enum  | [**Description**](#enum-description)  <br> |
| enum  | [**HandleInfoType**](#enum-handleinfotype)  <br> |
| enum  | [**LimitableResource**](#enum-limitableresource)  <br> |
| enum  | [**MemoryState**](#enum-memorystate)  <br> |
| enum  | [**ProcessInfoType**](#enum-processinfotype)  <br> |
| enum  | [**ResetType**](#enum-resettype)  <br> |
| typedef void(\* | [**ThreadFunc**](#typedef-threadfunc)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**\_NN\_OS\_RESULT\_DEF\_CONST**](#function-_nn_os_result_def_const) (ResultExceedTlsLimit, LEVEL\_PERMANENT, SUMMARY\_OUT\_OF\_RESOURCE, DESCRIPTION\_EXCEED\_TLS\_LIMIT) <br> |




























## Public Types Documentation




### enum ArbitrationType 

```C++
enum nn::os::ArbitrationType {
    ARBITRATION_TYPE_SIGNAL = 0,
    ARBITRATION_TYPE_WAIT_IF_LESS_THAN = 1,
    ARBITRATION_TYPE_DECREMENT_AND_WAIT_IF_LESS_THAN = 2,
    ARBITRATION_TYPE_WAIT_IF_LESS_THAN_WITH_TIMEOUT = 3,
    ARBITRATION_TYPE_DECREMENT_AND_WAIT_IF_LESS_THAN_WITH_TIMEOUT = 4,
    ARBITRATION_TYPE_MAX_BIT = 2147483648
};
```




<hr>



### enum Description 

```C++
enum nn::os::Description {
    DESCRIPTION_FAILED_TO_ALLOCATE_MEMORY = 1,
    DESCRIPTION_FAILED_TO_ALLOCATE_SHARED_MEMORY = 2,
    DESCRIPTION_FAILED_TO_ALLOCATE_THREAD = 3,
    DESCRIPTION_FAILED_TO_ALLOCATE_MUTEX = 4,
    DESCRIPTION_FAILED_TO_ALLOCATE_SEMAPHORE = 5,
    DESCRIPTION_FAILED_TO_ALLOCATE_EVENT = 6,
    DESCRIPTION_FAILED_TO_ALLOCATE_TIMER = 7,
    DESCRIPTION_FAILED_TO_ALLOCATE_PORT = 8,
    DESCRIPTION_FAILED_TO_ALLOCATE_SESSION = 9,
    DESCRIPTION_EXCEED_MEMORY_LIMIT = 10,
    DESCRIPTION_EXCEED_SHARED_MEMORY_LIMIT = 11,
    DESCRIPTION_EXCEED_THREAD_LIMIT = 12,
    DESCRIPTION_EXCEED_MUTEX_LIMIT = 13,
    DESCRIPTION_EXCEED_SEMAPHORE_LIMIT = 14,
    DESCRIPTION_EXCEED_EVENT_LIMIT = 15,
    DESCRIPTION_EXCEED_TIMER_LIMIT = 16,
    DESCRIPTION_EXCEED_PORT_LIMIT = 17,
    DESCRIPTION_EXCEED_SESSION_LIMIT = 18,
    DESCRIPTION_MAX_HANDLE = 19,
    DESCRIPTION_INACCESSIBLE_PAGE = 20,
    DESCRIPTION_ABANDONED = 21,
    DESCRIPTION_INVALID_PROCESS_ID = 24,
    DESCRIPTION_INVALID_THREAD_ID = 25,
    DESCRIPTION_SESSION_CLOSED = 26,
    DESCRIPTION_INVALID_MESSAGE = 28,
    DESCRIPTION_MANUAL_RESET_EVENT_REQUIRED = 29,
    DESCRIPTION_TOO_LONG_NAME = 30,
    DESCRIPTION_NOT_OWNED = 31,
    DESCRIPTION_PROCESS_TERMINATED = 32,
    DESCRIPTION_INVALID_TLS_INDEX = 33,
    DESCRIPTION_NO_RUNNABLE_PROCESSOR = 34,
    DESCRIPTION_NO_SESSION = 35,
    DESCRIPTION_USING_REGION = 36,
    DESCRIPTION_ALREADY_RECEIVED = 37,
    DESCRIPTION_CANCEL_REQUESTD = 38,
    DESCRIPTION_NOT_RECEIVED = 39,
    DESCRIPTION_DELIVER_ARG_NOT_READY = 41,
    DESCRIPTION_DELIVER_ARG_OVER_SIZE = 42,
    DESCRIPTION_INVALID_DELIVER_ARG = 43,
    DESCRIPTION_I_AM_OWNER = 44,
    DESCRIPTION_EXCEEDS_SHARED_LIMIT = 45,
    DESCRIPTION_UNEXPECTED_PERMISSION = 46,
    DESCRIPTION_INVALID_TAG = 47,
    DESCRIPTION_INVALID_FORMAT = 48,
    DESCRIPTION_OTHER_HANDLE = 49,
    DESCRIPTION_FAILED_TO_ALLOCATE_ADDRESS_ARBITER = 50,
    DESCRIPTION_EXCEED_ADDRESS_ARBITER_LIMIT = 51,
    DESCRIPTION_OVER_PORT_CAPACITY = 52,
    DESCRIPTION_NOT_MAPPED = 53,
    DESCRIPTION_NO_ADDRESS_SPACE = 55,
    DESCRIPTION_EXCEED_TLS_LIMIT = 56,
    DESCRIPTION_OBSOLETE_RESULT = 1023
};
```




<hr>



### enum HandleInfoType 

```C++
enum nn::os::HandleInfoType {
    HANDLE_INFO_TYPE_CREATION_TIME = 0,
    HANDLE_INFO_TYPE_REFERENCE_COUNT = 1,
    HANDLE_INFO_TYPE_PARENT_PROCESS_ID = 2,
    HANDLE_INFO_TYPE_MAX_BIT = 2147483648
};
```




<hr>



### enum LimitableResource 

```C++
enum nn::os::LimitableResource {
    LIMITABLE_RESOURCE_MAX_PRIORITY = 0,
    LIMITABLE_RESOURCE_MAX_COMMIT = 1,
    LIMITABLE_RESOURCE_MAX_THREAD = 2,
    LIMITABLE_RESOURCE_MAX_EVENT = 3,
    LIMITABLE_RESOURCE_MAX_MUTEX = 4,
    LIMITABLE_RESOURCE_MAX_SEMAPHORE = 5,
    LIMITABLE_RESOURCE_MAX_TIMER = 6,
    LIMITABLE_RESOURCE_MAX_SHAREDMEMORY = 7,
    LIMITABLE_RESOURCE_MAX_ADDRESSARBITER = 8,
    LIMITABLE_RESOURCE_MAX_CPUTIME = 9,
    LIMITABLE_RESOURCE_END = 10,
    LIMITABLE_RESOURCE_MAX_BIT = 2147483648
};
```




<hr>



### enum MemoryState 

```C++
enum nn::os::MemoryState {
    MEMORY_STATE_FREE = 0,
    MEMORY_STATE_RESERVED = 1,
    MEMORY_STATE_IO = 2,
    MEMORY_STATE_STATIC = 3,
    MEMORY_STATE_CODE = 4,
    MEMORY_STATE_PRIVATE = 5,
    MEMORY_STATE_SHARED = 6,
    MEMORY_STATE_CONTINUOUS = 7,
    MEMORY_STATE_ALIASED = 8,
    MEMORY_STATE_ALIAS = 9,
    MEMORY_STATE_ALIAS_CODE = 10,
    MEMORY_STATE_LOCKED = 11,
    MEMORY_STATE_MAX_BITS = 2147483648
};
```




<hr>



### enum ProcessInfoType 

```C++
enum nn::os::ProcessInfoType {
    PROCESS_INFO_TYPE_USING_PHYSICAL_MEMORY_SIZE = 0,
    PROCESS_INFO_TYPE_MAX_USING_PHYSICAL_MEMORY_SIZE = 1,
    PROCESS_INFO_TYPE_PRIVATE_PHYSICAL_MEMORY_SIZE = 2,
    PROCESS_INFO_TYPE_MAX_RPIVATE_PHYSICAL_MEMORY_SIZE = 3,
    PROCESS_INFO_TYPE_NUM_HANDLES = 4,
    PROCESS_INFO_TYPE_MAX_NUM_HANDLES = 5,
    PROCESS_INFO_TYPE_NUM_CREATED_THREADS = 6,
    PROCESS_INFO_TYPE_NUM_THREADS = 7,
    PROCESS_INFO_TYPE_MAX_NUM_THREADS = 8,
    PROCESS_INFO_TYPE_CPU_TIME_SYSTEM = 9,
    PROCESS_INFO_TYPE_CPU_TIME_USER = 10,
    PROCESS_INFO_TYPE_CPU_TIME = 11,
    PROCESS_INFO_TYPE_NUM_THREAD_SWITCH = 12,
    PROCESS_INFO_TYPE_NUM_FPU_SWITCH = 13,
    PROCESS_INFO_TYPE_NUM_PROCESS_SWITCH = 14,
    PROCESS_INFO_TYPE_NUM_SYSTEM_CALL = 15,
    PROCESS_INFO_TYPE_NUM_IPC = 16,
    PROCESS_INFO_TYPE_UPTIME = 17,
    PROCESS_INFO_TYPE_NAME = 18,
    PROCESS_INFO_TYPE_REGION = 19,
    PROCESS_INFO_TYPE_DEVICE_ADDRESS_OFFSET = 20,
    PROCESS_INFO_TYPE_WRAM_ADDRESS_OFFSET = 21,
    PROCESS_INFO_TYPE_WRAM_ADDRESS = 22,
    PROCESS_INFO_TYPE_WRAM_SIZE = 23,
    PROCESS_INFO_TYPE_MAX_BIT = 2147483648
};
```




<hr>



### enum ResetType 

```C++
enum nn::os::ResetType {
    RESET_TYPE_ONESHOT = 0,
    RESET_TYPE_STICKY = 1,
    RESET_TYPE_PULSE = 2,
    RESET_TYPE_MAX_BIT = 2147483648
};
```




<hr>



### typedef ThreadFunc 

```C++
typedef void(* nn::os::ThreadFunc) (uptr);
```




<hr>
## Public Functions Documentation




### function \_NN\_OS\_RESULT\_DEF\_CONST 

```C++
nn::os::_NN_OS_RESULT_DEF_CONST (
    ResultExceedTlsLimit,
    LEVEL_PERMANENT,
    SUMMARY_OUT_OF_RESOURCE,
    DESCRIPTION_EXCEED_TLS_LIMIT
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/os/CTR/os_CppException.h`

