# Quiz 005
## Solution
```.py
# Take the input
n1 = int(input("Please enter number:"))

# Make a list for factors
factors = []

limit = 1

# Make a loop to calculate the factors
while n1+1 != limit:
    if n1%limit == 0:
        factors.append(limit)
        limit = limit + 1
    else:
        limit = limit + 1
print(factors)
```

## Tests
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/quiz%205%20tests.png)
