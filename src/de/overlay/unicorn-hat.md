<!--
---
name: Unicorn HAT
manufacturer: Pimoroni
url: http://shop.pimoroni.com/products/unicorn-hat
buy: http://shop.pimoroni.com/products/unicorn-hat
description: 64 blendend helle RGB LEDs auf einem HAT
github: https://github.com/pimoroni/unicornhat
install:
  'apt':
    - 'python-dev'
    - 'python3-dev'
  'python':
    - 'unicornhat'
  'python3':
    - 'unicornhat'
  'examples': 'python/examples/'
pincount: 40
pin:
  '12':
    name: Data
    direction: output
    mode: pwm
    active: high
    description: WS2812 Data
-->
#Unicorn HAT

64 blendend helle LEDs auf einem HAT, die über eine super schnelle C-Library angesteuert werden.
Die C-Library lässt sich auch über Python ansteuern. Der Unicorn HAT ist quasi der grössere und hellere Bruder der PiGlow.

Hinweis: der Unicorn HAT trickst ein wenig mit dem PWM-Ausgang - der gleichen Hardware, mit der Dein Pi Sounds über den
analogen Audio-Ausgang erzeugen kann. Somit kannst Du nicht beides gleichzeitig nutzen!

Die Einrichtung des HATs ist einfach:

```bash
curl get.pimoroni.com/unicornhat | bash
```

Dann musst Du die Library nur noch in Dein Python-Skript importieren und kannst anfangen zu experimentieren:

```bash
import unicornhat
unicornhat.set_pixel(0, 0, 255, 255, 255)
unicornhat.show()
```