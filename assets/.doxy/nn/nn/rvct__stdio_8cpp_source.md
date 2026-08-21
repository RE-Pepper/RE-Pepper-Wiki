

# File rvct\_stdio.cpp

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**rtport**](dir_53d6a9bf16b96d25f9c91e79a4c5362a.md) **>** [**rvct**](dir_00ebb32c10ea47286a1d484d586cc083.md) **>** [**rvct\_stdio.cpp**](rvct__stdio_8cpp.md)

[Go to the documentation of this file](rvct__stdio_8cpp.md)


```C++
#include <cstring>
#include <nn/assert.h>
#include <nn/os/CTR/os_ThreadLocalRegion.h>
#include <rt_misc.h>
#include <rt_sys.h>
#include <typeinfo>

extern "C" {
const char __stdin_name[]  = "";
const char __stdout_name[] = "";
const char __stderr_name[] = "";

FILEHANDLE _sys_open(const char* name, int openmode)
{
        return -1;
} // 39
int _sys_close(FILEHANDLE fh)
{
        return -1;
} // 40
int _sys_write(FILEHANDLE fh, const unsigned char* buf, unsigned int len, int mode)
{
        return -1;
} // 41
int _sys_read(FILEHANDLE fh, unsigned char* buf, unsigned int len, int mode)
{
        return len;
} // 42
int _sys_istty(FILEHANDLE fh)
{
        return -1;
} // 44
int _sys_seek(FILEHANDLE fh, long pos)
{
        return -1;
} // 45

long _sys_flen(FILEHANDLE fh)
{
        return -1;
} // 47

void __rt_raise(int sig, int type) // 55
{
        RP_SHUTUP
}

void abort() // 58
{
        NN_PANIC_SDK("abort() called\n");
}

void __aeabi_atexit(void* object, void (*destructor)(void*), void* dso_handle) // 67
{
        RP_SHUTUP
}

void __rt_div0() // 71
{
        RP_SHUTUP
}

void** __rt_eh_globals_addr() // 74
{
        return &nn::os::CTR::GetThreadLocalRegion()->ehGlobalsAddr;
}

namespace std {
bool type_info::operator==(const type_info& rhs) const
{
        return std::strcmp(this->name(), rhs.name()) == 0;
}
bool type_info::operator!=(const type_info& rhs) const
{
        return std::strcmp(this->name(), rhs.name()) != 0;
}
bool type_info::before(const type_info& rhs) const
{
        return std::strcmp(this->name(), rhs.name()) < 0;
}
} // namespace std

} // extern "C"
```


