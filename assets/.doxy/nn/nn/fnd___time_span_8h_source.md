

# File fnd\_TimeSpan.h

[**File List**](files.md) **>** [**CtrSDK**](dir_a581c965070d8303a3ac233c6039c11a.md) **>** [**include**](dir_af9254bf4d22366cfccd04cbaa9622aa.md) **>** [**nn**](dir_a185e92459882a1d3c4a0e5724303e75.md) **>** [**fnd**](dir_896b02bd9724af022fac6ecc9927c6e1.md) **>** [**fnd\_TimeSpan.h**](fnd___time_span_8h.md)

[Go to the documentation of this file](fnd___time_span_8h.md)


```C++
#pragma once

namespace nn {
namespace fnd {

class TimeSpan
{
private:
        s64 m_NanoSeconds;
        typedef const struct ZeroOnlyTag
        {
        }* ZeroOnly;

public:
        TimeSpan (ZeroOnly zero = 0) : m_NanoSeconds ((s64)zero)
        {}
        // Creating
        static TimeSpan FromNanoSeconds (s64 nanoSeconds)
        {
                TimeSpan ret;
                ret.m_NanoSeconds = nanoSeconds;
                return ret;
        }
        static TimeSpan FromMicroSeconds (s64 microSeconds)
        {
                return FromNanoSeconds (microSeconds * 1000);
        }
        static TimeSpan FromMilliSeconds (s64 milliSeconds)
        {
                return FromNanoSeconds (milliSeconds * 1000 * 1000);
        }
        static TimeSpan FromSeconds (s64 seconds)
        {
                return FromNanoSeconds (seconds * 1000 * 1000 * 1000);
        }
        static TimeSpan FromMinutes (s64 minutes)
        {
                return FromNanoSeconds (minutes * 1000 * 1000 * 1000 * 60);
        }
        static TimeSpan FromHours (s64 hours)
        {
                return FromNanoSeconds (hours * 1000 * 1000 * 1000 * 60 * 60);
        }

        // Getting/Converting
        s64 GetNanoSeconds () const
        {
                return m_NanoSeconds;
        }
        s64 GetMicroSeconds () const
        {
                return m_NanoSeconds / 1000;
        }
        s64 GetMilliSeconds () const
        {
                return m_NanoSeconds / (1000 * 1000);
        }
        s64 GetSeconds () const
        {
                return m_NanoSeconds / (1000 * 1000 * 1000);
        }
        s64 GetMinutes () const
        {
                return m_NanoSeconds / (1000LL * 1000 * 1000 * 60);
        }
        s64 GetHours () const
        {
                return m_NanoSeconds / (1000LL * 1000 * 1000 * 60 * 60);
        }

        // Checking
        friend bool operator== (const TimeSpan& lhs, const TimeSpan& rhs)
        {
                return lhs.m_NanoSeconds == rhs.m_NanoSeconds;
        }
        friend bool operator!= (const TimeSpan& lhs, const TimeSpan& rhs)
        {
                return lhs.m_NanoSeconds != rhs.m_NanoSeconds;
        }
        friend bool operator< (const TimeSpan& lhs, const TimeSpan& rhs)
        {
                return lhs.m_NanoSeconds < rhs.m_NanoSeconds;
        }
        friend bool operator> (const TimeSpan& lhs, const TimeSpan& rhs)
        {
                return lhs.m_NanoSeconds > rhs.m_NanoSeconds;
        }
        friend bool operator<= (const TimeSpan& lhs, const TimeSpan& rhs)
        {
                return lhs.m_NanoSeconds <= rhs.m_NanoSeconds;
        }
        friend bool operator>= (const TimeSpan& lhs, const TimeSpan& rhs)
        {
                return lhs.m_NanoSeconds >= rhs.m_NanoSeconds;
        }

        // Modifying
        TimeSpan& operator+= (const TimeSpan& rhs)
        {
                this->m_NanoSeconds += rhs.m_NanoSeconds;
                return *this;
        }
        TimeSpan& operator-= (const TimeSpan& rhs)
        {
                this->m_NanoSeconds += rhs.m_NanoSeconds;
                return *this;
        }
        TimeSpan& operator*= (const TimeSpan& rhs)
        {
                this->m_NanoSeconds *= rhs.m_NanoSeconds;
                return *this;
        }
        TimeSpan& operator/= (const TimeSpan& rhs)
        {
                this->m_NanoSeconds /= rhs.m_NanoSeconds;
                return *this;
        }

        friend TimeSpan operator+ (const TimeSpan& lhs, const TimeSpan& rhs)
        {
                TimeSpan retval = FromNanoSeconds (lhs.m_NanoSeconds);
                retval.m_NanoSeconds += rhs.m_NanoSeconds;
                return retval;
        }
        friend TimeSpan operator- (const TimeSpan& lhs, const TimeSpan& rhs)
        {
                TimeSpan retval = FromNanoSeconds (lhs.m_NanoSeconds);
                retval.m_NanoSeconds -= rhs.m_NanoSeconds;
                return retval;
        }
};
static_assert_ (sizeof (TimeSpan) == 0x8);

} // namespace fnd
} // namespace nn
```


