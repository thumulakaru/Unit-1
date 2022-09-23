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

## 
