

# File os\_ResultFailureHandler.cpp

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**os**](dir_56153499d95e77076f83f9f8405b15c2.md) **>** [**os\_ResultFailureHandler.cpp**](os___result_failure_handler_8cpp.md)

[Go to the documentation of this file](os___result_failure_handler_8cpp.md)


```C++
#include <nn/Result.h>

RP_SHUTUP

void nnosGetProcessId(bit32* pOut) // 23
{
        // TODO
}

namespace {
void nnosResultFailureHandlerImplDefault(nnResult result, const char* filename, int lineno, const char* fmt, va_list vlist) // 60
{
        // TODO
}
void nnosResultTFailureHandlerImplDefault(nnResult result, const char* filename, int lineno, const char* fmt, ...) // 60
{
        // TODO
}

void nnosResultPanicHandlerImplDefault(nnResult result, const char* filename, int lineno, const char* fmt, va_list vlist) // 66
{
        bit32 processId;
        // TODO
}
void nnosResultTPanicHandlerImplDefault(nnResult result, const char* filename, int lineno, const char* fmt, ...) // 84
{
        bit32 processId;
        // TODO
}
} // namespace

int nnResultTFailureHandler(nnResult result, const char* filename, int lineno, const char* fmt, ...)
{
        va_list __va_list;
        return 0;
        // TODO
}
```


