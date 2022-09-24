# Lists
## Even Indices
```.py
a = input()
b = a.split(" ")

for i in range(0, len(b), 2):
    print(b[i])
```

## Even elements
```.py
a = input()
b = a.split(" ")

for i in range(len(b)):
    num = int(b[i])
    if abs(num%2) == 0:
        print(num)
```

## Greater than previous
```.py
a = [int(i) for i in input().split() ]
prev = a[0]
for c in range(0, len(a)):
    if prev < a[c]:
        print(a[c])
    prev = a[c]
```

## Neighbours of the same sign
```.py

```
