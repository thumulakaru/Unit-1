# Strings
## Slices
```.py
a = input()
print(a[2])
print(a[-2])
print(a[0:5])
print(a[0:-2])
print(a[0:len(a):2])
print(a[1:len(a):2])
print(a[::-1])
print(a[::-2])
print(len(a))
```

## The number of words
```.py
a = input()
print(a.count(" ")+1)
```

## The two halves
```.py
a = input()

b = a[0 : len(a)//2 + len(a)%2]
c = a[len(a)//2 + len(a)%2 : len(a)+1]
print(c+b)
```

## To swap the two words
```.py
a = input()
b = a.split()
a = ""

for i in range(len(b)-1, -1, -1):
    a = a + b[i]
    a = a + " "

print(a)
```

## The first and last occurrence
```.py
a = input()

b = a.find("f")
c = a.rfind("f")

if b != -1 or c != -1:
    if c == b:
        print(b)
    elif c == -1:
        print(b)
    else:
        print(str(b) + " " + str(c))
```

## Second Occurrence
```.py
s = input()
с = s.count('f')
if с == 0:
    print(-2)
if с == 1:
    print(-1)
if с > 1:
    print(s.find('f', s.find('f') + 1))
```

## Remove the fragment
```.py
a = input()
print(a[:a.find('h')] + a[a.rfind('h')+1:])
```

## Reverse the fragment
```.py
a = input()
i = a[a.find('h'):(a.rfind('h'))]
print(a[:a.find('h') + 1] + i[::-1] + a[a.rfind('h')+1:])
```

## Replace the substring
```.py
a = input()
print(a.replace("1", "one"))
```

## Delete a character
```.py
a = input()
print(a.replace("@",""))
```

## Replace within the fragment
```.py
a = input()

b = a[a.find("h")+1 : a.rfind("h")]

print(a[:a.find("h") + 1] + b.replace("h", "H") + a[a.rfind("h"):])
```

## Delete every third character
```.py
a = input()
b = ""

for i in range(0, len(a)):
    c = i%3
    if c == 0:
        b = b
    else:
        b = b + a[i]
print(b)
```
