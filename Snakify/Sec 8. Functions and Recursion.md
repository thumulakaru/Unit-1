## The length of segment
```.py
from math import sqrt
def distance(a1, b1, a2, b2:float)->float:
    d = sqrt((a2-a1)**2 + (b2-b1)**2)
    return d

print(distance(float(input()), float(input()), float(input()), float(input())))
```

## Negative exponent
```.py
def power(a:float, n:int)->float:
    out = a ** n
    return out
print(power(float(input()), int(input())))
```

## Uppercase
```.py
def capitalize(lower_case_word):
    out = ""
    if lower_case_word.count(" ") != 0:
        a = lower_case_word.split()
        for b in range(0, len(a)):
            for i in range(0, len(a[b])):
                if i == 0:
                    out += chr(ord((a[b])[i])-32)
                else:
                    out += ((a[b])[i])
            out += " "
    else:
        for i in range(0, len(lower_case_word)):
            if i == 0:
                out = chr(ord(lower_case_word[i])-32)
            else:
                out += lower_case_word[i]
    return out
print(capitalize(input()))
```

## Exponentiation
```.py
def power(a, n):
    if n == 0:
        b = 1
    else:
        b = a * power(a, n-1)
    return b
print(power(float(input()), int(input())))
```

## Reverse the sequence
```.py
def reverse():
    a = int(input())
    if a != 0:
        reverse()
    print(a)

reverse()
```

## Fibonacci numbers
```.py
def fib(n):
    if n == 1 or n == 2:
        b = 1
        return b
    else:
        b = fib(n-1)+(fib(n-2))
        return b
print(fib(int(input())))
```
