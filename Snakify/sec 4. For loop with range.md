# For loop with range

## Count to N
```.py
n = int(input())
for i in range(1,n+1):
    print(i)
```

## Series - 1
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

## Series - 2
```.py
a = int(input())
b = int(input())


if a < b:
    for x in range(a, b+1):
        print(x)
elif a > b:
    for x in range(a , b-1, -1):
        print(x)
    
else:
    print(a)
```

## First N even, descending
```.py
n = int(input())
if n%2==0:
    for i in range(n,-1,-2):
        print(i)
else:
    n = n-1
    for i in range(n,-1,-2):
        print(i)
```

## Sum of ten numbers
```.py
i = int(input())
count = 1
while count != 10:
    i = i + int(input())
    count = count+1

print(i)
```

## Sum of N numbers
```.py
x = int(input())
count = 1
if x != 0:
    i = int(input())
    while count != x:
        i = i + int(input())
        count = count+1
    print(i)
elif x == 0:
    print(0)
```

## Product of N numbers
```.py
max = int(input())
a = 1

for i in range(max):
    a = int(input())*a

print(a)
```

## Sum of cubes
```.py
max = int(input())
max = max+1
t = 0
for i in range(0, max):
    t = i**3 + t
print(t)
```

## Factorial 
```.py
a = int(input())
t = 1
for i in range(1, a+1):
    t = i*t
print(t)
```

## The number of zeros
```.py
max = int(input())
count = 0

for i in range(max):
    b = int(input())
    if b == 0:
        count = count + 1

print(count)
```

## Adding factorials
```.py
a = int(input())
t = 1
out = 0
for i in range(1, a+1):
    t = i*t
    out = t + out
print(out)
```

## Squares in range
```.py
a = int(input())
b = int(input())

for i in range(a, b+1):
    print(i,i, sep="*", end="=")
    print(i*i)
```

## Ladder
```.py
a = int(input())
b = ""
for i in range(1, a+1):
    c = str(i)
    b = b + c
    print(b)
```

## Is prime
```.py
a = int(input())
count = 0

for i in range(1, a+1):
    b = a%i
    if b == 0:
        count = count+1

if count == 2:
    print("PRIME")
else:
    print("COMPOSITE")
```

## Print primes in range
```.py
a = int(input())
b = int(input())

for x in range(a, b+1):
    count = 0
    for i in range(2, x):
        if x%i == 0:
            count = 1
    if count == 0:
        print(x)
```

## Number of primes in range
```.py
a = int(input())
b = int(input())
h = 0

for x in range(a, b+1):
    count = 0
    for i in range(2, x):
        if x%i == 0:
            count = 1
    if count == 0:
        h = h+1
print(h)
```

## Lost Card
```.py
answer = 0
N= int(input())
b = N
for i in range(N-1):
  N = int(input())
  answer = answer + N
for i in range(b):
  b = i + b
  i = N + i
b = abs(answer - b)
print(b)
```
