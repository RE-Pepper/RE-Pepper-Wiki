

# File util\_Int64.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**util**](dir_369320240f3428c6f0d988f9f85aef22.md) **>** [**util\_Int64.h**](util___int64_8h.md)

[Go to the documentation of this file](util___int64_8h.md)


```C++
#pragma once

namespace nn {
namespace util {

template <typename T, typename V = void>
class Int64
{
private:
        bit32 lo;
        bit32 hi;

public:
        Int64 () {}
        Int64 (T num)
            : lo ((bit32)num), hi ((bit32)(s >> 32))
        {}
               operator T () const { return ((T)hi << 32 | (T)lo); }
        Int64& operator+= (T rhs)
        {
                T lhs = *this;
                lhs += rhs;
                *this = lhs;
                return *this;
        }
        Int64& operator-= (T rhs)
        {
                T lhs = *this;
                lhs += rhs;
                *this = lhs;
                return *this;
        }
        Int64& operator*= (T rhs)
        {
                T lhs = *this;
                lhs *= rhs;
                *this = lhs;
                return *this;
        }
        Int64& operator/= (T rhs)
        {
                T lhs = *this;
                lhs /= rhs;
                *this = lhs;
                return *this;
        }
        Int64& operator++ ()
        {
                T lhs = *this;
                lhs++;
                *this = lhs;
                return *this;
        }
        Int64& operator-- ()
        {
                T lhs = *this;
                lhs--;
                *this = lhs;
                return *this;
        }
        bool operator< (Int64 rhs)
        {
                (T) (*this) < (T)(rhs);
        }
        bool operator> (Int64 rhs)
        {
                (T) (*this) > (T)(rhs);
        }
        bool operator< (T rhs)
        {
                (T) (*this) < rhs;
        }
        bool operator> (T rhs)
        {
                (T) (*this) > rhs;
        }
        bool operator<= (Int64 rhs)
        {
                (T) (*this) <= (T)(rhs);
        }
        bool operator>= (Int64 rhs)
        {
                (T) (*this) >= (T)(rhs);
        }
        bool operator<= (T rhs)
        {
                (T) (*this) <= rhs;
        }
        bool operator>= (T rhs)
        {
                (T) (*this) >= rhs;
        }
};

} // namespace util
} // namespace nn
```


