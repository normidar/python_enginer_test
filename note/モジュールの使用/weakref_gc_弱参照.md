# コードをご覧

```
# 自動参照確認のdictが作れる
import weakref
# メモリーの掃除を行う
import gc

class Objj:
    pass

# 参照を作る
a = Objj() # or some other object
d = weakref.WeakValueDictionary()
d["a"] = a
print(d["a"])

# 参照を削除
del a
gc.collect()
print(d["a"]) # エラーになる

```

