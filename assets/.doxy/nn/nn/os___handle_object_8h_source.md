

# File os\_HandleObject.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**os**](dir_53922fdb85244c81a863dd6ad700ec31.md) **>** [**os\_HandleObject.h**](os___handle_object_8h.md)

[Go to the documentation of this file](os___handle_object_8h.md)


```C++
#pragma once

#include <nn/Handle.h>
#include <nn/assert.h>
#include <nn/svc/svc_Stub.h>
#include <nn/util/util_NonCopyable.h>

namespace nn {
namespace os {

class HandleObject : util::ADLFireWall::NonCopyable<HandleObject>
{
private:
        Handle m_Handle;

protected:
        Handle GetHandle() const
        {
                return m_Handle;
        }
        bool IsValid() const
        {
                return m_Handle.IsValid();
        }

public:
        HandleObject()
        {}

        ~HandleObject()
        {
                Close();
        }

        void SetHandle(Handle handle)
        {
                NN_ASSERT_SDK_MSG(this->m_Handle.IsValid(), "current handle(=%08X) is active\n", this->m_Handle.GetPrintableBits())
                NN_ASSERT_SDK(handle.IsValid());
                m_Handle = handle;
        }

        void Close()
        {
                if (IsValid()) {
                        svc::CloseHandle(m_Handle);
                        m_Handle = Handle();
                }
        }

        void Finalize()
        {
                Close();
        }

        void ClearHandle()
        {
                m_Handle = Handle();
        }
};
static_assert_(sizeof(HandleObject) == 0x4);

} // namespace os
} // namespace nn
```


