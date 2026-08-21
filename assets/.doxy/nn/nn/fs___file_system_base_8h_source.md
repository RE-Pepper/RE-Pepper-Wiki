

# File fs\_FileSystemBase.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**fs**](dir_ebaeb7c8987009097a9882ca30046667.md) **>** [**fs\_FileSystemBase.h**](fs___file_system_base_8h.md)

[Go to the documentation of this file](fs___file_system_base_8h.md)


```C++
#pragma once

#include <nn/fs/CTR/MPCore/fs_UserFileSystem.h>

namespace nn {
namespace fs {
namespace detail {

class FileSystemBaseImpl : public CTR::MPCore::detail::UserFileSystem
{
};

class FileSystemBase
{
private:
        FileSystemBaseImpl m_pImpl;

public:
        FileSystemBase ();

        void   Initialize (FileSystemBaseImpl*);
        Result TryDeleteFile (const char*);
        Result TryRenameFile (const char*, const char*);
        Result TryCreateFile (const char*, s64);
        Result TryCreateDirectory (const char*);
};

class WPathBuffer
{
private:
        wchar_t m_pBuffer[270];

public:
        WPathBuffer (const char*);
};

} // namespace detail
} // namespace fs
} // namespace nn
```


