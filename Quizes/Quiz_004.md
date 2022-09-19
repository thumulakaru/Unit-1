# Quiz 4
## Solution
```.py
# Take the input
n1 = int(input("Please enter number:"))

# Make a list for factors
factors = []

# Add a variable to check limit
limit = 1

# Make a loop to calculate the factors
while n1!= limit:
    if n1%limit == 0:
        factors.append(limit)
        limit = limit + 1
    else:
        limit = limit + 1

if sum(factors) == n1:
    print("Is perfect")
else:
    print("Not perfect")
    print(sum(factors))
```

## Tests
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz%204%20tests.png)

## Flow diagram
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz_004_FlowDiagram.jpg)
