

# File util\_FlagsEnum.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**util**](dir_369320240f3428c6f0d988f9f85aef22.md) **>** [**util\_FlagsEnum.h**](util___flags_enum_8h.md)

[Go to the documentation of this file](util___flags_enum_8h.md)


```C++
#pragma once

namespace nn {
namespace os {

template <typename T, typename V>
class FlagsEnum
{
private:
        T m_FlagsValue;

public:
        FlagsEnum () {}
        FlagsEnum (T e) : m_FlagsValue (e) {}
        FlagsEnum (V e) : m_FlagsValue (e) {}

        T    Get () const { return this->m_FlagsValue; }
        void Set (T e) const { this->m_FlagsValue = e; }

        operator T () { return Get (); }
};

template <typename V>
struct FlagsEnum1 : public FlagsEnum<bit8, V>
{
        FlagsEnum1 () : FlagsEnum<bit8, V> () {}
        FlagsEnum1 (V e) : FlagsEnum<bit8, V> (e) {}
};
template <typename V>
struct FlagsEnum2 : public FlagsEnum<bit16, V>
{
        FlagsEnum2 () : FlagsEnum<bit16, V> () {}
        FlagsEnum2 (V e) : FlagsEnum<bit16, V> (e) {}
};
template <typename V>
struct FlagsEnum4 : public FlagsEnum<bit32, V>
{
        FlagsEnum4 () : FlagsEnum<bit32, V> () {}
        FlagsEnum4 (V e) : FlagsEnum<bit32, V> (e) {}
};

} // namespace os
} // namespace nn
```


