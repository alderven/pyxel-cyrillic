# pyxel-cyrillic
Cyrillic font for python pyxel

Currently [pyxel](https://github.com/kitao/pyxel) [doesn't support](https://github.com/kitao/pyxel/issues/126) cyrillic font. This is workaround script for using cyrillic font.

![](https://github.com/alderven/pyxel-cyrillic/blob/master/alphabet.png?raw=true)

Some symbols may absent. Feel free to add it yourself.

### Sample usage:
```
import pyxel
import pyxelcyrillic

pyxel.init(200, 160)

def update():
    if pyxel.btnp(pyxel.KEY_Q):
        pyxel.quit()

def draw():
    pyxel.cls(0)
    pyxelcyrillic.text('Привет, мир!', 75, 80, 8)

pyxel.run(update, draw)
```

![](https://github.com/alderven/pyxel-cyrillic/blob/master/hello_world.png?raw=true)
