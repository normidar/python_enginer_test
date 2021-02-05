
# デフォルトは６つを出力　「大事」

> 簡単

```
import reprlib
reprlib.repr(set('diveintocode'))
# >>> "{'c', 'd', 'e', 'i', 'n', 'o', ...}"
```

> 詳しい

```
import reprlib
r = reprlib.Repr()
r.maxlist = 4       # max elements displayed for lists
r.maxstring = 10    # max characters displayed for strings

obj = [[1, 2, 3], list(range(10000)), 'looooooong string', 'a', 'b', 'c']

print(r.repr(obj))
# >>> [[1, 2, 3], [0, 1, 2, 3, ...], 'lo...ing', 'a', ...]
```
