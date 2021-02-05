# プログラム実は二進数を使っておりよく十進数の計算を間違えてしまう。

```
from decimal import *
print(Decimal('1.00') % Decimal('.10'))
print(1.00 % 0.10)
```
