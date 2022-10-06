# Quiz 15
## Solution
```.py
def num_open_doors(num_students:int):
    num_doors = num_students
    status = [True, False]
    doors_status = []
    for i in range(num_doors):
        doors_status.append(False)
    for d in range(1, num_doors+1):
        for stu in range(1, num_students+1):
            if d % stu == 0:
                doors_status[d-1] = not doors_status[d-1]
    out = doors_status.count(True)
    return out


num_student_in = int(input("Please enter the number of students:"))
print(num_open_doors(num_student_in))
```

## Flow diagrams
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz_015_FlowDiagram_part1.png)

![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz_015_FlowDiagram_part2.png)

## Tests
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz%2015%20tests.png)
