

# File module.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**module.h**](module_8h.md)

[Go to the documentation of this file](module_8h.md)


```C++
#pragma once

#include <nn/util/detail/util_Symbol.h>

#define NN_MAKE_MODULE(Variable, Company, Module) \
        const char Variable[] __attribute__((section(".module_id"))) = "[SDK+" Company ":" Module "]"

#define NN_MAKE_MODULE_SDK(Variable, Module) \
        NN_MAKE_MODULE(Variable, "NINTENDO", Module)

#define NN_REFER_MODULE(Variable) \
        nnutilReferSymbol_(Variable)
```


