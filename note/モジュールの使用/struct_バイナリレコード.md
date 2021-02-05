
> オブジェクトを２進数データに転換するのをバイナリレコードという。（ちなみに中国語では序列化という）序列化

```
from struct import *
data = pack('hhl', 1, 2, 3)
# type(data) # >>> bytes
unpack('hhl', data)
# >>> (1,2,3)
```
