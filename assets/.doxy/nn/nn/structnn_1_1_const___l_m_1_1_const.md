

# Struct nn::Const\_LM::Const

**template &lt;[**Result::Summary**](classnn_1_1_result.md#enum-summary) TSummary, int TDescription&gt;**



[**ClassList**](annotated.md) **>** [**nn**](namespacenn.md) **>** [**Const\_LM**](structnn_1_1_const___l_m.md) **>** [**Const**](structnn_1_1_const___l_m_1_1_const.md)





* `#include <Result.h>`



Inherits the following classes: [nn::Result::Const](structnn_1_1_result_1_1_const.md)


















## Public Types inherited from nn::Result

See [nn::Result](classnn_1_1_result.md)

| Type | Name |
| ---: | :--- |
| enum  | [**Description**](classnn_1_1_result.md#enum-description)  <br> |
| enum  | [**Level**](classnn_1_1_result.md#enum-level)  <br> |
| enum  | [**Module**](classnn_1_1_result.md#enum-module)  <br> |
| enum  | [**Summary**](classnn_1_1_result.md#enum-summary)  <br> |


























































## Public Functions inherited from nn::Result::Const

See [nn::Result::Const](structnn_1_1_result_1_1_const.md)

| Type | Name |
| ---: | :--- |
|   | [**Const**](structnn_1_1_result_1_1_const.md#function-const) () <br> |


## Public Functions inherited from nn::Result

See [nn::Result](classnn_1_1_result.md)

| Type | Name |
| ---: | :--- |
|  [**bit32**](types_8h.md#typedef-bit32) | [**GetCodeBits**](classnn_1_1_result.md#function-getcodebits) ([**bit32**](types_8h.md#typedef-bit32) mask, [**s32**](types_8h.md#typedef-s32) shift) const<br> |
|  int | [**GetDescription**](classnn_1_1_result.md#function-getdescription) () const<br> |
|  [**Level**](classnn_1_1_result.md#enum-level) | [**GetLevel**](classnn_1_1_result.md#function-getlevel) () const<br> |
|  [**Module**](classnn_1_1_result.md#enum-module) | [**GetModule**](classnn_1_1_result.md#function-getmodule) () const<br> |
|  [**bit32**](types_8h.md#typedef-bit32) | [**GetPrintableBits**](classnn_1_1_result.md#function-getprintablebits) () const<br> |
|  [**Summary**](classnn_1_1_result.md#enum-summary) | [**GetSummary**](classnn_1_1_result.md#function-getsummary) () const<br> |
|  bool | [**IsFailure**](classnn_1_1_result.md#function-isfailure) () const<br> |
|  bool | [**IsSuccess**](classnn_1_1_result.md#function-issuccess) () const<br> |
|   | [**Result**](classnn_1_1_result.md#function-result-14) ([**bit32**](types_8h.md#typedef-bit32) code) <br> |
|   | [**Result**](classnn_1_1_result.md#function-result-24) () <br> |
|   | [**Result**](classnn_1_1_result.md#function-result-34) ([**Level**](classnn_1_1_result.md#enum-level) level, [**Summary**](classnn_1_1_result.md#enum-summary) summary, [**Module**](classnn_1_1_result.md#enum-module) module, int description) <br> |
|   | [**Result**](classnn_1_1_result.md#function-result-44) ([**nnResult**](structnn_result.md) result) <br> |
|   | [**operator nnResult**](classnn_1_1_result.md#function-operator-nnresult) () <br> |
|  bool | [**operator!=**](classnn_1_1_result.md#function-operator) (const [**Result**](classnn_1_1_result.md) & rhs) <br> |
|  bool | [**operator==**](classnn_1_1_result.md#function-operator_1) (const [**Result**](classnn_1_1_result.md) & rhs) <br> |
























## Protected Attributes inherited from nn::Result

See [nn::Result](classnn_1_1_result.md)

| Type | Name |
| ---: | :--- |
|  [**bit32**](types_8h.md#typedef-bit32) | [**m\_Code**](classnn_1_1_result.md#variable-m_code)  <br> |

























































------------------------------
The documentation for this class was generated from the following file `lib/CtrSDK/include/nn/Result.h`

