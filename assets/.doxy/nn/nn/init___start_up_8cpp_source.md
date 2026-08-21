

# File init\_StartUp.cpp

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**sources**](dir_6ad72fc0abbc32b2f59992fddd21f3c1.md) **>** [**libraries**](dir_80d58af41f6b82f04b97d791f7cfcb5d.md) **>** [**init**](dir_c7386c615566c444dc954695d2e7bbc4.md) **>** [**init\_StartUp.cpp**](init___start_up_8cpp.md)

[Go to the documentation of this file](init___start_up_8cpp.md)


```C++
#include <nn/init/init_StartUp.h>

RP_SHUTUP

extern "C" void nninitSystem () // 43
{
        // nn::os::Initialize();
#if 0
        // nn::srv::Initialize();
#endif
}

extern "C" void nninitSetupDaemons () // 55
{
        // nn::ndm::SetupDaemonsDefault();
}

extern "C" nninitStaticInitFunc Image$$STATIC_INIT$$RO$$Base[];
extern "C" nninitStaticInitFunc Image$$STATIC_INIT$$RO$$Limit[];

extern "C" void nninitCallStaticInitializers () // 62
{
        for (nninitStaticInitFunc* f = Image$$STATIC_INIT$$RO$$Base;
                f < Image$$STATIC_INIT$$RO$$Limit;
                ++f) {
                (*f) ();
        }
}

extern "C" void nninitSetup () // 72
{
        /*
        nninitSetupDefault();
        nn::os::CTR::defaul::SetInternalErrorHandlingMode(0); // TODO MACRO
        nn::applet::CTR::detaul::Initialize(0); // TODO MACRO
        nninitSetupDaemons();
        */
}
```


