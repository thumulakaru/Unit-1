# Conditions if, then, else
## Is Positive
```.py
a = int(input())
if a > 0:
    print("YES")
elif a<0:
    print("NO")
else:
    print("You entered zero")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-05%20at%2010.06.42.png)

## Is Odd
```.py
a = int(input())

if a%2==1:
    print("YES")
elif a%2==0:
    print("NO")
else:
    print("You entered an invalid input.")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-05%20at%2020.59.29.png)

## Is Even
```.py
a = int(input())

if a%2==0:
    print("YES")
elif a%2==1:
    print("NO")
else:
    print("You entered an invalid input.")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-05%20at%2021.02.23.png)
## Ends on Seven
```.py
a = int(input())
if a%10 == 7:
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-05%20at%2021.06.15.png)

## Minimum of two numbers
```.py
a = int(input())
b = int(input())

if a > b:
    print(b)
else:
    print(a)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2011.51.41.png)

## Are both odd
```.py
a = int(input())
b = int(input())

if a%2 == 1 and b%2 == 1:
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-05%20at%2021.11.20.png)

## At least one odd
```.py
a = int(input())
b = int(input())

if a%2 == 1 or b%2 == 1:
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-05%20at%2021.38.15.png)

## Exactly one odd
```.py
a = int(input())
b = int(input())

if (a%2==1 and b%2==0) or (a%2==0 and b%2==1):
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-06%20at%2013.30.47.png)

## Sign function
```.py
a = int(input())
if a>0:
    print("+1")
elif a==0:
    print(0)
else:
    print("-1")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2012.10.20.png)

## Numbers in ascending order
```.py
a = int(input())
b = int(input())
c = int(input())

if c>b and b>a:
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-06%20at%2013.36.05.png)

## Is three digit
```.py
a = int(input())

if a//100>=1 and a//100<10:
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-06%20at%2013.38.53.png)

## Minimum of three numbers
```.py
a = int(input())
b = int(input())
c = int(input())
if a<b and a<c:
    print(a)
elif a<b and a>c:
    print(c)
elif b<a and b<c:
    print(b)
elif b<a and b>c:
    print(c)
else:
    print(a)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2020.55.36.png)

## Equal numbers
```.py
a = int(input())
b = int(input())
c = int(input())

if a!=b and a!=c and b!=c:
    print(0)
elif a==b and a==c:
    print(3)
elif a==b and a!=c:
    print(2)
elif c==b and a!=c:
    print(2)
else:
    print(2)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2021.00.17.png)

## Rook move

```.py
a = int(input())
b = int(input())
c = int(input())
d = int(input())
if a == c and b!= d:
    print("YES")
elif a != c and b ==d:
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2021.08.50.png)
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2021.08.59.png)

## Chess Board - Black Square
```.py
a = int(input())
b = int(input())

if (a+b)%2==0:
    print("BLACK")
else:
    print("WHITE")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-06%20at%2013.42.37.png)
## Chess Board - Same Colour
```.py
a = int(input())
b = int(input())
c = int(input())
d = int(input())

e = ((a+b)%2)
f = ((c+d)%2)

if e==f:
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2021.15.37.png)

## Distance to the closest point
```.py
a = int(input())
b = int(input())
c = int(input())

ab = abs(a-b)
ac = abs(a-c)

if ab<ac:
    print(ab)
else:
    print(ac)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-07%20at%2018.57.49.png)

## Digits in ascending order
```.py
a = int(input())

h = a//100
t = (a%100)//10
o = (a%100)%10

if o>t and t>h and o>h:
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-07%20at%2018.55.20.png)

## Four digit pallandrome
```.py
a = int(input())

f = str(a//1000)
s = str((a%1000)//100)
t = str(((a%1000)%100)//10)
l = str(a%10)

b = int(l+t+s+f)


if a == b:
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-07%20at%2019.08.29.png)

## King move

```.py
a = int(input())
b = int(input())
c = int(input())
d = int(input())

if a == c+1 and (b == d or b==d+1 or b==d-1):
    print("YES")
elif a == c-1 and (b == d or b==d+1 or b==d-1):
    print("YES")
elif a == c and (b == d+1 or b == d-1):
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2021.22.11.png)
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2021.23.12.png)

## Bishop move
```.py
a1=int(input())
a2=int(input())
b1=int(input())
b2=int(input())
if abs(a1-b1)==abs(a2-b2):
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2021.51.17.png)
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2021.51.32.png)

## Queen move
```.py
a1=int(input())
a2=int(input())
b1=int(input())
b2=int(input())
if abs(a1-b1)==abs(a2-b2):
    print("YES")
elif (a1 == b1 and a2!= b2) or (a1 != b1 and a2 ==b2):
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2022.00.05.png)

## Index of outlier
```.py
a = int(input())
b = int(input())
c = int(input())

if a == b:
    print("3")
elif b == c:
    print("1")
else:
    print("2")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-07%20at%2019.11.46.png)

## Knight Move
```.py
a = int(input())
b = int(input())
c = int(input())
d = int(input())

if ((a+1)==c or (a-1)==c) and (b == d+2 or b==d-2):
    print("YES")
elif ((a+2)==c or (a-2)==c) and (b== d+1 or b == d-1):
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2022.52.19.png)

## Chocolate Bar

```.py
n = int(input())
m = int(input())
k = int(input())
s = n*m
if ((k%n)==0 or (k%m)==0) and (s>=k):
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2023.01.06.png)

## Leap Year

```.py
a = int(input())
if (a%400 == 0):
    print("LEAP")
elif (a%400 != 0 and a%100==0):
    print("COMMON")
elif (a%400 != 0 and a%100!=0 and a%4==0):
    print("LEAP")
else:
    print("COMMON")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-31%20at%2023.07.55.png)

## Days in month
```.py
a = int(input())

if a == 1 or a == 3 or a == 5 or a == 7 or a == 8 or a == 10 or a == 12:
    print("31")
elif a == 4 or a == 6 or a == 9 or a == 11:
    print("30")
else:
    print("28")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-07%20at%2019.15.22.png)

## Next day
```.py
a = int(input())
b = int(input())

if (b == 31 and (a == 1 or a == 3 or a == 5 or a == 7 or a == 8 or a == 10)) or (b == 30 and (a == 4 or a == 6 or a == 9 or a == 11)) or (b == 28 and a == 2) :
    a = a+1
    b = 1
    print(a)
    print(b)
elif b == 31 and a == 12:
    a = 1
    b = 1
    print(a)
    print(b)
elif (b != 31 and (a == 1 or a == 3 or a == 5 or a == 7 or a == 8 or a == 10 or a == 12)) or (b != 30 and (a == 4 or a == 6 or a == 9 or a == 11)) or (b != 28 and a == 2) :
    b = b+1
    print(a)
    print(b)
else:
    print("ERROR")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-07%20at%2019.24.20.png)

## Linear equation
```.py
a = int(input())
b = int(input())
g = ("no solution")
f = ("many solutions")

if a != 0 and b !=0:
    d1 = b/a
    d2 = b//a

    if d1 == d2:
        print(d1)
    else:
        print(g)
elif a == 0 and b != 0:
    print(g)
elif a != 0 and b == 0:
    print(g)
else:
    print(f)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-07%20at%2019.34.52.png)

## Vertices of rectangle
```.py
a1 = int(input())
a2 = int(input())
b1 = int(input())
b2 = int(input())
c1 = int(input())
c2 = int(input())
d1 = 0
d2 = 0
if a1==b1 or a1 == c1:
    if a1 == c1:
        d1 = b1
    else:
        d1 = c1
else:
    d1 = a1
if a2 == b2 or a2 == c2:
    if a2 == c2:
        d2 = b2
    else:
        d2 = c2
else:
    d2 = a2
    
print(d1)
print(d2)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-08%20at%208.59.58.png)

## Sort three numbers
```.py
a = int(input())
b = int(input())
c = int(input())

if a > b:
    if a>c:
        if b>c:
            print(c)
            print(b)
            print(a)
        else:
            print(b)
            print(c)
            print(a)
    else:
        print(b)
        print(a)
        print(c)
elif b>c:
    if c > a:
        print(a)
        print(c)
        print(b)
    else:
        print(c)
        print(a)
        print(b)
else:
    print(a)
    print(b)
    print(c)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-08%20at%209.11.16.png)

## Pawn move

```.py
ax = int(input())
ay = int(input())
bx = int(input())
by = int(input())

if ax == bx and ay+1==by and ay != 1:
    print("YES")
elif abs(ax-bx)==1 and ay+1 == by and ay != 1:
    print("YES")
elif ax == bx and ay+2 == by and ay == 2 and ay != 1:
    print("YES")
else:
    print("NO")
```

![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-08%20at%209.18.25.png)
