

# Class nn::fnd::TimeSpan



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**fnd**](namespacenn_1_1fnd.md) **>** [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md)





* `#include <fnd_TimeSpan.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**s64**](types_8h.md#typedef-s64) | [**GetHours**](#function-gethours) () const<br> |
|  [**s64**](types_8h.md#typedef-s64) | [**GetMicroSeconds**](#function-getmicroseconds) () const<br> |
|  [**s64**](types_8h.md#typedef-s64) | [**GetMilliSeconds**](#function-getmilliseconds) () const<br> |
|  [**s64**](types_8h.md#typedef-s64) | [**GetMinutes**](#function-getminutes) () const<br> |
|  [**s64**](types_8h.md#typedef-s64) | [**GetNanoSeconds**](#function-getnanoseconds) () const<br> |
|  [**s64**](types_8h.md#typedef-s64) | [**GetSeconds**](#function-getseconds) () const<br> |
|   | [**TimeSpan**](#function-timespan) ([**ZeroOnly**](classnn_1_1fnd_1_1_time_span.md#typedef-zeroonly) zero=0) <br> |
|  [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md) & | [**operator\*=**](#function-operator) (const [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md) & rhs) <br> |
|  [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md) & | [**operator+=**](#function-operator_1) (const [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md) & rhs) <br> |
|  [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md) & | [**operator-=**](#function-operator-) (const [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md) & rhs) <br> |
|  [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md) & | [**operator/=**](#function-operator_2) (const [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md) & rhs) <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md) | [**FromHours**](#function-fromhours) ([**s64**](types_8h.md#typedef-s64) hours) <br> |
|  [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md) | [**FromMicroSeconds**](#function-frommicroseconds) ([**s64**](types_8h.md#typedef-s64) microSeconds) <br> |
|  [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md) | [**FromMilliSeconds**](#function-frommilliseconds) ([**s64**](types_8h.md#typedef-s64) milliSeconds) <br> |
|  [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md) | [**FromMinutes**](#function-fromminutes) ([**s64**](types_8h.md#typedef-s64) minutes) <br> |
|  [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md) | [**FromNanoSeconds**](#function-fromnanoseconds) ([**s64**](types_8h.md#typedef-s64) nanoSeconds) <br> |
|  [**TimeSpan**](classnn_1_1fnd_1_1_time_span.md) | [**FromSeconds**](#function-fromseconds) ([**s64**](types_8h.md#typedef-s64) seconds) <br> |


























## Public Functions Documentation




### function GetHours 

```C++
inline s64 nn::fnd::TimeSpan::GetHours () const
```




<hr>



### function GetMicroSeconds 

```C++
inline s64 nn::fnd::TimeSpan::GetMicroSeconds () const
```




<hr>



### function GetMilliSeconds 

```C++
inline s64 nn::fnd::TimeSpan::GetMilliSeconds () const
```




<hr>



### function GetMinutes 

```C++
inline s64 nn::fnd::TimeSpan::GetMinutes () const
```




<hr>



### function GetNanoSeconds 

```C++
inline s64 nn::fnd::TimeSpan::GetNanoSeconds () const
```




<hr>



### function GetSeconds 

```C++
inline s64 nn::fnd::TimeSpan::GetSeconds () const
```




<hr>



### function TimeSpan 

```C++
inline nn::fnd::TimeSpan::TimeSpan (
    ZeroOnly zero=0
) 
```




<hr>



### function operator\*= 

```C++
inline TimeSpan & nn::fnd::TimeSpan::operator*= (
    const TimeSpan & rhs
) 
```




<hr>



### function operator+= 

```C++
inline TimeSpan & nn::fnd::TimeSpan::operator+= (
    const TimeSpan & rhs
) 
```




<hr>



### function operator-= 

```C++
inline TimeSpan & nn::fnd::TimeSpan::operator-= (
    const TimeSpan & rhs
) 
```




<hr>



### function operator/= 

```C++
inline TimeSpan & nn::fnd::TimeSpan::operator/= (
    const TimeSpan & rhs
) 
```




<hr>
## Public Static Functions Documentation




### function FromHours 

```C++
static inline TimeSpan nn::fnd::TimeSpan::FromHours (
    s64 hours
) 
```




<hr>



### function FromMicroSeconds 

```C++
static inline TimeSpan nn::fnd::TimeSpan::FromMicroSeconds (
    s64 microSeconds
) 
```




<hr>



### function FromMilliSeconds 

```C++
static inline TimeSpan nn::fnd::TimeSpan::FromMilliSeconds (
    s64 milliSeconds
) 
```




<hr>



### function FromMinutes 

```C++
static inline TimeSpan nn::fnd::TimeSpan::FromMinutes (
    s64 minutes
) 
```




<hr>



### function FromNanoSeconds 

```C++
static inline TimeSpan nn::fnd::TimeSpan::FromNanoSeconds (
    s64 nanoSeconds
) 
```




<hr>



### function FromSeconds 

```C++
static inline TimeSpan nn::fnd::TimeSpan::FromSeconds (
    s64 seconds
) 
```




<hr>## Friends Documentation





### friend operator!= 

```C++
inline bool nn::fnd::TimeSpan::operator!= (
    const TimeSpan & lhs,
    const TimeSpan & rhs
) 
```




<hr>



### friend operator+ 

```C++
inline TimeSpan nn::fnd::TimeSpan::operator+ (
    const TimeSpan & lhs,
    const TimeSpan & rhs
) 
```




<hr>



### friend operator- 

```C++
inline TimeSpan nn::fnd::TimeSpan::operator- (
    const TimeSpan & lhs,
    const TimeSpan & rhs
) 
```




<hr>



### friend operator&lt; 

```C++
inline bool nn::fnd::TimeSpan::operator< (
    const TimeSpan & lhs,
    const TimeSpan & rhs
) 
```




<hr>



### friend operator&lt;= 

```C++
inline bool nn::fnd::TimeSpan::operator<= (
    const TimeSpan & lhs,
    const TimeSpan & rhs
) 
```




<hr>



### friend operator== 

```C++
inline bool nn::fnd::TimeSpan::operator== (
    const TimeSpan & lhs,
    const TimeSpan & rhs
) 
```




<hr>



### friend operator&gt; 

```C++
inline bool nn::fnd::TimeSpan::operator> (
    const TimeSpan & lhs,
    const TimeSpan & rhs
) 
```




<hr>



### friend operator&gt;= 

```C++
inline bool nn::fnd::TimeSpan::operator>= (
    const TimeSpan & lhs,
    const TimeSpan & rhs
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/fnd/fnd_TimeSpan.h`

