# Sec 2. Integer and Float numbers
The first part of the problems were added separately.

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
