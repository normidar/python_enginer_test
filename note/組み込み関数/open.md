# open 関数はファイルを読み込んだり、書き込んだりする時に使います。

```
open(file, mode='r', buffering=-1, encoding=None, errors=None, newline=None, closefd=True, opener=None)
```

中のmodeは大事です。

> from head => overwrite

```
t デフォルト　ファイルモード
x write new file mode, will throw error when file exist
b byte mode,
+ open a file to update
r read only mode
rb read only and use byte mode
r+ open a file to read and write from head
rb+ read only and use byte mode from head
w open a file to write from head, while file not exist create new
wb open a file to write bytes, overwrite, create new
...
```

簡単に言えば：

```
w -> write
r -> read
a -> append
b -> bytes
+ -> write and read
```

