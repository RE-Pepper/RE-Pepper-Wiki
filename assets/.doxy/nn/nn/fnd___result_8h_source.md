

# File fnd\_Result.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**fnd**](dir_896b02bd9724af022fac6ecc9927c6e1.md) **>** [**fnd\_Result.h**](fnd___result_8h.md)

[Go to the documentation of this file](fnd___result_8h.md)


```C++
#pragma once

#include <nn/Result.h>

namespace nn {
namespace fnd {

enum Description
{
        DESCRIPTION_UNK1 = 1,
        DESCRIPTION_UNK2 = 2
};

#define _NN_FND_RESULT_DEF_CONST(result, level, summary, description) \
        NN_RESULT_DEF_CONST (result, Result::level, Result::summary, Result::MODULE_NN_FND, description)

_NN_FND_RESULT_DEF_CONST (ResultInvalidAddress, LEVEL_USAGE, SUMMARY_INVALID_ARGUMENT, Result::DESCRIPTION_INVALID_ADDRESS);

_NN_FND_RESULT_DEF_CONST (ResultFndUnk0, LEVEL_USAGE, SUMMARY_INVALID_ARGUMENT, DESCRIPTION_UNK2);

} // namespace fnd
} // namespace nn
```


