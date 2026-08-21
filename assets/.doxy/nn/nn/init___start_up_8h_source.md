

# File init\_StartUp.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**init**](dir_d55def94f65a12fb344229c5bcac0d9a.md) **>** [**init\_StartUp.h**](init___start_up_8h.md)

[Go to the documentation of this file](init___start_up_8h.md)


```C++
#pragma once

#ifdef __cplusplus
extern "C" {
#endif

typedef void (*nninitStaticInitFunc) ();

void nninitSystem ();
void nninitSetupDaemons ();
void nninitCallStaticInitializers ();
void nninitSetup ();

#ifdef __cplusplus
}
#endif
```


