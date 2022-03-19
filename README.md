# Hellow world
First hellow world example with pygame:

```python
import pygame, sys
from pygame.locals import *

pygame.init()
DISPLAYSURF = pygame.display.set_mode((400, 300))
pygame.display.set_caption('Hello World!')
while True: # main game loop
    for event in pygame.event.get():
        if event.type == QUIT:
            pygame.quit()
            sys.exit()
    pygame.display.update()
```
Notes:

Normally if you want to call a function that
is in a module, you must use the modulename.functionname() format after importing the
module. However, with from modulename import *, you can skip the modulename.
portion and simply use functionname() (just like Python’s built-in functions)

>resources/practice/[HelloWorld.py](https://github.com/badorius/pygame_course/blob/main/resources/practice/HelloWorld.py)
---
