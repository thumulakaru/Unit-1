## The length of segment
```.py
from math import sqrt
def distance(a1, b1, a2, b2:float)->float:
    d = sqrt((a2-a1)**2 + (b2-b1)**2)
    return d

print(distance(float(input()), float(input()), float(input()), float(input())))
```
