# Quiz002

## Solution to the SL problem
```.py
count = 1
while count!= 5:
    a = int(input("1:"))
    b = int(input("2:"))
    if a+b==20 or a==20 or b==20:
        c = True
        count = count + 1
        print(c)
    else:
        c = False
        count = count + 1
        print(c)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-09-01%20at%2019.31.38.png)
## Solution to the HL problem
```.py
l1 = []
l2 = []
c = False
count = 0

n = int(input("Enter the number of elements in the first list: "))
m = int(input("Enter the number of elements in the first list: "))

for i in range(0, n):
    a = int(input("Enter your number in list 1:"))
    l1.append(a)

for i in range(0, m):
    b = int(input("Enter your number in list 2:"))
    l2.append(b)

while not c:
    for i in range(0, n):
        if l1[i] == 20 or l2[i] == 20 or l1[i]+l2[i] == 20:
            c = True
            break
        else:
            c = False
            count = count + 1
print("The answer of this quiz is", c)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-09-01%20at%2019.25.18.png)
