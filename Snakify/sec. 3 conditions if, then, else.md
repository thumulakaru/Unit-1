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

## Are both odd
```.py
a = int(input())
b = int(input())

if a%2 == 1 or b%2 == 1:
    print("YES")
else:
    print("NO")
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screenshots%20from%2004.09.2022/Screen%20Shot%202022-09-05%20at%2021.38.15.png)

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

## Chess Board- Same Colour

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
