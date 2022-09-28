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
a = [int(s) for s in input().split()]
for i in range(1, len(a)):
    if a[i] * a[i-1] > 0:
        print(a[i-1], a[i], end=' ')
        break
```
## Greater than neighbours
```.py
a = [int(s) for s in input().split()]
count = 0
for i in range(1, len(a)-1):
    if a[i] > a[(i-1)] and a[i] > a[i+1]:
        count += 1
print(count)
```

## The largest element
```.py
a = [int(s) for s in input().split()]
max = a[0]-1
for i in range(0, len(a)):
    if a[i]>max:
        max = a[i]
        index = i
print(max)
print(index)
```

## The number of distinct elements
```.py
a = [int(s) for s in input().split()]
prev = a[0]
count = 1
for i in range(1, len(a)):
    if prev != a[i]:
        count += 1
        prev = a[i]
print(count)
```

## Swap neighbours
```.py
a = [int(s) for s in input().split()]
for i in range(0, len(a)-1, 2):
    a[i], a[i+1] = a[i+1], a[i]
out = ""
for b in a:
    out += str(b) + " "
print(out)
```

## Swap min and max
```.py
a = [int(s) for s in input().split() ]
min = a[0]
max = a[0]
min_index = 0
max_index = 0
for i in range(1, (len(a))):
    if a[i] < min:
        min = a[i]
        min_index = i
    elif a[i] > max:
        max = a[i]
        max_index = i

a[min_index], a[max_index] = a[max_index], a[min_index]

out = ""
for b in a:
    out += str(b) + " "
print(out)
```

## The number of pairs of equal
```.py
a = [int(s) for s in input().split()]
count = 0
for i in range(0, len(a)):
    for b in range(i+1, len(a)):
        if a[i] == a[b]:
            count += 1
print(count)
```

## Unique elements
```.py
a = [int(s) for s in input().split()]
out = []
for element in a:
    if a.count(element) == 1:
       out.append(element)
for el in out:
    print(el)
```

## Queens
```.py
num_of_queens = 8
result = 'NO'
x = [0] * num_of_queens
y = [0] * num_of_queens
for i in range(num_of_queens):
    x[i], y[i] = [int(b) for b in input().split()]
for i in range (num_of_queens):
    for c in range(i + 1, num_of_queens):
        if x[i] == x[c] or y[i] == y[c] or abs(x[i] - x[c]) == abs(y[i] - y[c]):
            result = 'YES'
print(result)
```

## The bowling alley
```.py
t, n = [int(i) for i in input().split()]
pins = ["I" for x in range(t)]
for i in range(n):
    a, b = [int(c) for c in input().split()]
    for j in range(a-1, b):
        pins[j] = '.'
print("".join(pins))        
```
