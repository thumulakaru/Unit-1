# Quiz 13

## Solution
```.py
def mystery(num1_in,num2_in:int)->int:
    if num1_in != num2_in:
        sub_num = abs(num1_in-num2_in)
    else:
        sub_num = num1_in
    out = (num1_in * num2_in)-sub_num
    return out

in1 = int(input("Please enter your 1st number:"))
in2 = int(input("Please enter your 2st number:"))
print(mystery(in1, in2))
```

## Tests
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz%2013%20tests.png)

## Flowcharts
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz_013_FlowDiagram.png)
