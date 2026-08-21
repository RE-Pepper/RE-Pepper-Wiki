

# File dbg\_PrintResult.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**dbg**](dir_8674e25a187048eae8b9b07d931da2b2.md) **>** [**dbg\_PrintResult.h**](dbg___print_result_8h.md)

[Go to the documentation of this file](dbg___print_result_8h.md)


```C++
#pragma once

#include <nn/Result.h>

#ifdef __cplusplus

namespace nn {
namespace dbg {
namespace detail {

void PrintResult (Result result);
void TPrintResult (Result result);

const char* GetLevelString (Result result);
const char* GetModuleString (Result result);
const char* GetSummaryString (Result result);
const char* GetDescriptionString (Result result);
const char* GetResultCommonDescriptionStringImpl (Result result);

} // namespace detail
} // namespace dbg
} // namespace nn

#endif
```


