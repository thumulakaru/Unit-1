# For loop with range

## Count to N
```.py
n = int(input())
for i in range(1,n+1):
    print(i)
```

## Series-1
```.py
a = int(input())
b = int(input())

for i in range(a,b+1):
    print(i)
```

## First N odd, ascending
```.py
a = int(input())

for i in range(1,a+1):
    if i%2 == 1:
        print(i)
```
