

# File Handle.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**Handle.h**](_handle_8h.md)

[Go to the documentation of this file](_handle_8h.md)


```C++
#pragma once

#ifdef __cplusplus
extern "C" {
#endif

typedef struct nnHandle
{
        bit32 value;
} nnHandle;

namespace {
const nnHandle INVALID_HANDLE_VALUE         = { 0x0 };
const nnHandle PSEUDO_HANDLE_CURRENT_THREAD = { 0xFFFF800 };
} // namespace

#ifdef __cplusplus
}
#endif

namespace nn {

class Handle
{
protected:
        bit32 m_Handle;

public:
        Handle ()
            : m_Handle (0)
        {}
        Handle (nnHandle handle)
            : m_Handle (handle.value)
        {}
        Handle (bit32 value)
            : m_Handle (value)
        {}

        bool IsValid () const
        {
                return this->m_Handle != 0;
        }

        bit32 GetPrintableBits () const
        {
                return this->m_Handle;
        }

        bool operator== (const Handle& rhs) const { return this->m_Handle == rhs.m_Handle; }
        bool operator!= (const Handle& rhs) const { return this->m_Handle != rhs.m_Handle; }
             operator nnHandle () const
        {
                nnHandle result = { m_Handle };
                return result;
        }
};

} // namespace nn

```


