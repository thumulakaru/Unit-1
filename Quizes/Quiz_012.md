# Quiz 12

## Solution
```.py
user_num_in = int(input("Please enter a number between 2 and 10:"))
def mulTable(num_in:int)->str:
    out = ("")
    for i in range(2, 10):
        temp = i * num_in
        ans = num_in*1
        out += (f"{num_in} x {i} = {temp}\n")
    return out

print(mulTable(user_num_in))
```

## Tests
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz%2012%20tests.png)

## Flow Diagram
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz_012_FlowDiagram.png)
