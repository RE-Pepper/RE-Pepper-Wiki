

# File cfg\_UserInfo.h

[**File List**](files.md) **>** [**cfg**](dir_d61dd7901f361aace8efbc35eb1e8191.md) **>** [**CTR**](dir_6286be2e3839b9d14dbaf851f98cbdb4.md) **>** [**cfg\_UserInfo.h**](cfg___user_info_8h.md)

[Go to the documentation of this file](cfg___user_info_8h.md)


```C++
#pragma once

namespace nn {
namespace cfg {
namespace CTR {

struct UserName
{
        wchar_t userName[11];
        bool    isNgUserName;
};
static_assert_ (sizeof (UserName) == 0x18);

struct Birthday
{
        s8 month;
        s8 day;
};
static_assert_ (sizeof (Birthday) == 0x2);

struct SimpleAddress
{
        u32 id;

        wchar_t countryName[64];
        wchar_t regionName[16];

        u16 latitude;
        u16 longitude;
};
static_assert_ (sizeof (SimpleAddress) == 0xA8);

} // namespace CTR
} // namespace cfg
} // namespace nn
```


