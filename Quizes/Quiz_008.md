# Quiz 008
## Solution
```.py
# Defining a function
def roomnum(a:int)->str:
    room_num = a%10
    floor_num = a//10
    if room_num == 0:
        room_num = 10
    else:
        floor_num = floor_num + 1
    floor_num =str(floor_num)
    room_num = str(room_num)
    print(f"Room {floor_num}F-{room_num} ")

v = int(input("Please enter the number:"))
roomnum(v)
```

## Tests
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz%208%20tests.png)

**Figure 1:** Tests for the problem
