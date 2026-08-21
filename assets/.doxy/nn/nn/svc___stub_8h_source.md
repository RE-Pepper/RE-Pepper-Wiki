

# File svc\_Stub.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**svc**](dir_c1b0279480f3283373e7c3eb28175a75.md) **>** [**svc\_Stub.h**](svc___stub_8h.md)

[Go to the documentation of this file](svc___stub_8h.md)


```C++
#pragma once

#include <nn/Handle.h>
#include <nn/Result.h>
#include <nn/os/os_SvcTypes.autogen.h>
#include <nn/os/os_Types.h>
#include <nn/svc/svc_Stub.h>

namespace nn {
namespace svc {

Result ControlMemory (uptr* addr, uptr addr0, uptr addr1, size_t size, u32 op, u32 perms);
Result QueryMemory(nn::os::MemoryInfo* mem, nn::os::PageInfo* page, u32);
void   ExitProcess ();
void   CreateThread (Handle* handle, void (*func) (u32), u32 arg, u32 stackTop, s32 prio, s32 processorId);
void   SleepThread (u64 nanos);
Result GetThreadPriority (s32* prio, Handle thread);
Result SetThreadPriority (Handle thread, int prio);
u32    GetCurrentProcessorNumber ();
Result CreateMutex (Handle* mutex, bool initialLocked);
Result ReleaseMutex (Handle mutex);
Result CreateEvent (Handle* event, nn::os::ResetType type);
Result SignalEvent (Handle event);
Result ClearEvent (Handle mutex);
Result CreateMemoryBlock (Handle* memblock, u32 addr, u32 size, u32 myperms, u32 otherperms);
Result MapMemoryBlock (Handle block, u32 i0, u32 start, u32 end);
Result UnmapMemoryBlock (Handle block, u32 i0);
Result CreateAddressArbiter (Handle* arbiter);
Result ArbitrateAddress (Handle arbiter, uptr addr, nn::os::ArbitrationType type, s32 value);
Result CloseHandle (Handle handle);
Result WaitSynchronizationN (int* pOut, const Handle* handles, s32 handleCount, bool waitAll, s64 timeout_ns);
Result WaitSynchronization1 (int* pOut, s64 timeout_ns);
Result DuplicateHandle (Handle* pOut, Handle original);
u32    GetSystemTick ();
Result GetProcessInfo(u64* num, Handle handle, nn::os::ProcessInfoType infoType);
Result ConnectToPort (Handle* port, const char* portName);
Result SendSyncRequest (Handle handle);
Result GetProcessId (u32* id, Handle handle);
Result GetThreadId (u32* id, Handle handle);
Result GetResourceLimit (Handle* resourceLimit, Handle handle);
} // namespace svc
} // namespace nn
```


