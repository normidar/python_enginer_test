
# テンプレート（神社じゃない）

> テンプレートとはformatと似たような機能を持つ、string文字列に何かを入れることに使う。

```
from string import Template
s = Template('$who likes $what')
s.substitute(who='tim', what='kung pao')
# >>> 'tim likes kung pao'
```
