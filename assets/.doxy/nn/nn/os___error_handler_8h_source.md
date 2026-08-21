

# File os\_ErrorHandler.h

[**File List**](files.md) **>** [**CTR**](dir_58d889e92b967b98a0adfbe142d43dad.md) **>** [**os\_ErrorHandler.h**](os___error_handler_8h.md)

[Go to the documentation of this file](os___error_handler_8h.md)


```C++
#pragma once

#include <nn/Result.h>

namespace nn {
namespace os {
namespace CTR {
namespace detail {

void HandleInternalError(Result result, const char* filename, int lineno);
void HandleInternalError(Result result);

void SetInternalErrorHandlingMode(bool preferFatal);

#if NN_SWITCH_DISABLE_DEBUG_PRINT_FOR_SDK == 1
#define NN_OS_HANDLE_ERROR(result)                                      \
        Result nn_os_result = (result);                                 \
        if (nn_os_result.IsFailure()) {                                 \
                nn::os::CTR::detail::HandleInternalError(nn_os_result); \
        }
#else
#define NN_OS_HANDLE_ERROR(result)                                                               \
        Result nn_os_result = (result);                                                          \
        if (nn_os_result.IsFailure()) {                                                          \
                nn::os::CTR::detail::HandleInternalError(nn_os_result, __BASE_FILE__, __LINE__); \
        }
#endif

} // namespace detail
} // namespace CTR
} // namespace os
} // namespace nn
```


