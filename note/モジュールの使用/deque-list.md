# deque

### importの仕方

```
from collections import deque
```

### 関数

```
append(item)
appendleft(item)
pop()
popleft()
```

# list

```
sort(cmp=None,key=None,reverse=False)
reverse　は下がるかどうかを決定するパラメータ、Falseだと上る順で。

key の使い方：

def takeSecond(elem):
    return elem[1]

lst = [(2, 2), (3, 4), (4, 1), (1, 3)]

lst.sort(key=takeSecond)

>>> [(4, 1), (2, 2), (1, 3), (3, 4)]  # 二番目見て、のぼる順でsortされた。
```