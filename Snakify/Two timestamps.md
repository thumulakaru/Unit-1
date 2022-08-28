# Two timestamps
## Solution to the problem

```.py
h1 = int(input("Please enter the number of hours:"))
m1 = int(input("Please enter the number of minutes:"))
s1 = int(input("Please enter the number of seconds:"))

h1 = (h1 * 3600)
m1 = (m1 * 60)
t1 = (h1+m1+s1)

h2 = int(input("Please enter the number of hours:"))
m2 = int(input("Please enter the number of minutes:"))
s2 = int(input("Please enter the number of seconds:"))

h2 = (h2 * 3600)
m2 = (m2 * 60)
t2 = (h2+m2+s2)

ans = (t2-t1)
print(ans)
```
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-08-28%20at%2022.49.23.png)

**Figure 1** The tests
