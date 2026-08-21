

# File cfg\_ParentalControl.h

[**File List**](files.md) **>** [**cfg**](dir_d61dd7901f361aace8efbc35eb1e8191.md) **>** [**CTR**](dir_6286be2e3839b9d14dbaf851f98cbdb4.md) **>** [**cfg\_ParentalControl.h**](cfg___parental_control_8h.md)

[Go to the documentation of this file](cfg___parental_control_8h.md)


```C++
#pragma once

namespace nn {
namespace cfg {
namespace CTR {

struct ParentalControlFlags
{
        u32 isSetParentalControl;
        u32 browser;
        u32 ulcd;
        u32 photoExchange;
        u32 p2pInternet;
        u32 p2pCec;
        u32 addFriend;
        u32 dsDownload;
        u32 shopPoint;
        u32 video;
        u32 rsv;
};
static_assert_ (sizeof (ParentalControlFlags) == 0x2C);

struct ParentalControlInfo
{
        ParentalControlFlags flags;

        u32  rsv1;
        u8   ogn;
        u8   ratingAge;
        u8   secretQuestionID;
        u8   secretAnswerLength;
        char password[5];
        u8   rsv2[3];

        wchar_t secretAnswer[65];

        u8 rsv3[42];
};
static_assert_ (sizeof (ParentalControlInfo) == 0xE8);

} // namespace CTR
} // namespace cfg
} // namespace nn
```


