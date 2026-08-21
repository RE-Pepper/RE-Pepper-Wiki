

# File fs\_ParametersForSystem.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**fs**](dir_ebaeb7c8987009097a9882ca30046667.md) **>** [**fs\_ParametersForSystem.h**](fs___parameters_for_system_8h.md)

[Go to the documentation of this file](fs___parameters_for_system_8h.md)


```C++
#pragma once

#include <nn/fs/fs_Parameters.h>
#include <nn/util/util_SizedEnum.h>

namespace nn {
namespace fs {

struct WriteOption
{
        bool flush;
        bool updateTimeStampOld;
        bool updateTimeStamp;
        bit8 reserved3;

        WriteOption (bool flush, bool updateTimeStamp)
            : flush (flush), updateTimeStampOld (false), updateTimeStamp (updateTimeStamp)
        {}
};

typedef bit32 SystemSaveDataId; // 70

typedef bit32 ContentIdx; // 74

typedef struct TitleDataSpecifier
{
        TitleId                     id;
        util::SizedEnum1<MediaType> media;
        // two unnamed ints?
        int unk0;
        int unk1;

        static TitleDataSpecifier Make (MediaType type, TitleId id)
        {
                TitleDataSpecifier ret;
                ret.id    = id;
                ret.media = type;
                return ret;
        }
} ProgramLaunchInfo; // 98

enum SystemMediaType
{
        SYSTEM_MEDIA_TYPE_CTR_NAND,
        SYSTEM_MEDIA_TYPE_TWL_NAND,
        SYSTEM_MEDIA_TYPE_SDMC,
        SYSTEM_MEDIA_TYPE_TWL_PHOTO
};

} // namespace fs
} // namespace nn
```


