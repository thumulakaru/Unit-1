# While loop
## List of squares
```.py
N = int(input())
i = 1
while i**2 <= N:
    print(i**2)
    i += 1
```

## Least divisor
```.py
a = int(input())
b = 2

while a%b != 0:
    b += 1

print(b)
```

## The power of two
```.py
n = int(input())
a = 2
count = 0


while n >= a:
    a = a*2
    count += 1

print(count)
print(a/2)
```

## Morning jog
```.py
x = int(input())
y = int(input())
day = 1

while y > x:
    x = x * 110/100
    day = day+1

print(day)
```

## The length of sequence
```.py
a = False
count = 0
while a == False:
    b = int(input())
    if b != 0:
        count += 1
    else:
        a = True

print(count)
```

## The sum of the sequence
```.py
sum = 0
a = False
while a == False:
    b = int(input())
    if b != 0:
        sum = sum + b
    else:
        a = True
print(sum)
```

## The average of the sequence
```.py
sum = 0
element = 0
a = False
while a == False:
    b = int(input())
    if b != 0:
        sum = sum + b
        element = element + 1
    else:
        a = True
print(sum/element)
```

## The maximum of the sequnce
```.py
b = 1
max = 0
while b != 0:
    b = int(input())
    if b > max:
        max = b

print(max)
```

## The index of the maximum of the sequence
```.py
b = 1
max = 0
count = 0
while b != 0:
    b = int(input())
    count = count + 1
    if b > max:
        max = b
        maxcount = count

print(maxcount)
```

## The number of even elements of the sequence
```.py
a = int(input())
count = 0
while a != 0:
    if a%2 == 0:
        count += 1
    a = int(input())
print(count)
```

## The number of elements that are greater than the previous one
```.py
a = int(input())
count = 0
b = int(input())
while b != 0:
    if a < b:
        count += 1
    a = b
    b = int(input())
print(count)
```

## The second maximum
```.py
a = 0
b = int(input())
max = 0
while b != 0:
    if max < b:
        a = max
        max = b
    elif a < b:
        a = b
    b = int(input())
print(a)
```

## The number of elements equal to the maximum
```.py
max = 0
count = 1
a = int(input())
while a != 0:
    if a > max:
        max = a
        count = 1
    elif a == max:
        count += 1
    a = int(input())
print(count)
```

## Fibonacci number
```.py
n = int(input())
fi1 = 0
fi2 = 1
if n < 1:
    print(0)
elif n == 1:
    print(1)
else:
    i = 2
    while i <= n:
        fi2, fi1 = fi1 + fi2, fi2
        i += 1
    print(fi2)
```

## The index of a fiboniacci number
```.py
A = int(input())
fi1 = 0
fi2 = 1
if A == 1:
    print(1)
else:
    i = 1
    while A > fi2:
        fi2, fi1 = fi1 + fi2, fi2
        i += 1
    if A == fi2:
        print(i)
    else:
        print(-1)
```

## The maximum number of consecutive equal numbers
```.py
count = 1
max_count = 1
a = int(input())
b = a
while b != 0:
    b, a = int(input()), b
    if b == a:
        count += 1
    else:
        if count > max_count:
            max_count = count
        count = 1
print(max_count)
```
