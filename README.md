### bidict
---
https://github.com/jab/bidict

```py
from bidict import bidict
element_by_symbol = bidict({'H': 'hydrogen'})
element_by_symbol['H']
element_by_symbol.inverse['hydrogen']


from bidict import RAISE, OVERWRITE, IGNORE
b = bidict({2: 4})
b.put(2, 8, on_dup_key=RAISE)
b
b.putall([(3, 9), (2, 8)], on_dup_key=RAISE)
b
b.putall([(3, 9), (1, 4)], on_dup_val=IGNORE)

b = bidict({0: 0, 1: 2})
b.forceupdate([(2, 0), (0, 1), (0, 0)])
sorted(b.items())
b = bidict({0: 0, 1: 2})
b.forceupdate([(0, 1), (0, 0), (2, 0)])
sorted(b.items())
```

```
```

```
```


