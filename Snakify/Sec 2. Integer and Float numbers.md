# Sec 2. Integer and Float numbers
The first part of the problems were added separately.

## Last Two Digits
```.py
a = int(input())
print(a%100)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-09-01%20at%2019.35.04.png)

## Reverse Three Digits
```.py
a = int(input())

e = str(a//100)
f = str((a%100)//10)
g = str(a%10)
print(g+f+e)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2011.36.11.png)

## Merge two numbers
```.py
a = int(input())
b = int(input())

c = str(a//10)
d = str(a%10)
e = str(b//10)
f = str(b%10)

print(c+e+d+f)
```

## Cyclic Rotation
```.py
a = int(input())

b = str(a//100)
c = str(a%100)
print(c+b)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-09-01%20at%2020.00.42.png)

## Fractional part
```.py
a = float(input())
b = int(a)
b = a-b
print(b)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-09-01%20at%2019.57.38.png)

## First digit after decimal point

```.py
b = float(input())
a = (int((b*10)%10))
print(a)
```

![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-30%20at%2013.11.15.png)
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-30%20at%2013.12.42.png)

## Car route

```.py
N = int(input())
M = int(input())
d = (M//N)
r = (M%N)
if d==0:
    print(1)
elif d>= 1 and r!=0:
    print(d+1)
elif d>=1 and r==0:
    print(d)
else:
    print("1")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-30%20at%2013.32.07.png)

## Day of week
```.py
i = int(input())
print((i+3)%7)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-04%20at%2020.52.55.png)

## Digital clock
```.py
a = int(input())

h = str(a//60)
m = str(a%60)

print(h,m)
```

![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-30%20at%2013.37.00.png)

## Total cost
```.py
a = int(input())
b = int(input())
n = int(input())

ad = (a*100+b)
tc = (n*ad)

d = (str(tc//100))
c = (str(tc%100))

print(d, c)
```

![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-30%20at%2013.48.47.png)

## Century
```.py
from math import ceil

x = int(input())
x = (x/100)
print(ceil(x))
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-04%20at%2021.05.00.png)

## Snail
```.py
from math import ceil

a = int(input())
b = int(input())
c = int(input())

print(ceil((a-b)/(b-c))+1)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-04%20at%2021.13.12.png)

## Clock Face - 1
```.py
h = int(input())
m = int(input())
s = int(input())

hand = (((h*3600+m*60+s)/43200)*360)

print(hand)
```

![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-30%20at%2014.14.54.png)

## Clock face - 2
```.py
a = float(input())
a = (a%30)*12
print(a)
```

![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-04%20at%2021.14.49.png)
