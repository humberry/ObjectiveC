# ObjectiveC<br>

### Data Types<br>

| data type | value | ctype | python | value |
| :---: | :---: | :---: | :---: | :---: |
| BOOL | YES / NO | c_bool | bool | True / False |
| char | e.g. 'a' | c_char | byte object | e.g. 97 |
| short int | -32.768 … 32.767 | c_short | int | e.g. 32000 |
| unsigned short int | 0 … 65.535 | c_ushort | int | e.g. 65000 |
| int | -2.147.483.648 … 2.147.483.647 | c_int | int | e.g. 2000000000 |
| unsigned int | 0 … 4.294.967.295 | c_uint | int | e.g. 4000000000 |
| long int | -9.223.372.036.854.775.808 … 9.223.372.036.854.775.807 | c_long | int | e.g. 9000000000000000000 |
| unsigned long int | 0 … 18.446.744.073.709.551.615 | c_ulong | int | ... |
| float | 4 bytes as in int values | c_float | float | ... |
| double | 8 bytes as in long int values | c_double | float | ... |
| void | no value | c_void_p | int or None | no value |
| \*pointer | memory address | POINTER(c_int) or byref(obj) | - | - |

[Pythonista ctypes](http://omz-software.com/pythonista/docs/library/ctypes.html)<br>
[Objective-C data types 1](https://code.tutsplus.com/tutorials/objective-c-succinctly-data-types--mobile-21986)<br>
[Objective-C data types 2](https://www.tutorialspoint.com/objective_c/objective_c_data_types)<br>

[Apple Developer Documentation](https://developer.apple.com/documentation/)<br>
Language: Objective-C<br>

```python
# set screen brightness to 60%
from objc_util import *
ObjCClass('UIScreen').mainScreen().setBrightness(0.6)

# ObjCClass('UIScreen') => interface => type: NSObject
# mainScreen() => property of UIScreen
# setBrightness(0.6) => property of mainScreen => type: CGFloat (0.0 ... 1.0)

# see also Pythonista => Examples => ObjC => ScreenBrightness.py
```

External link disclaimer:<br>
I'm not responsible for the content of external websites.<br>
