# Quiz 010
## Solution
```.py
#2022-09-22 Quiz 010

#Create a function that produces the powers of ten from pico to tera for a number provided as an input parameter. The function should return a list of the powers of ten.
#HL: User inputs number with units (e.g. 1 gram of salt)
s = input("Input a number with unit: ")
n = [int(s) for s in s.split() if s.isdigit()]
powers = []
units = ["Tera", "Giga", "Mega", "Kilo", "Unit", "Milli", "Micro", "Nano", "Pico"]
ljust_length = 20


def power(n):
    count = 0
    for i in range(-12, 0, 3):
        temp = abs(i // 3)
        number = f"0.{(('000 ') * temp)}{str(n[0])} ".ljust(ljust_length)
        powers.append(f"{number}{units[count]}{s[1:]}")
        count += 1
    for i in range(0, 15, 3):
        temp = i//3
        number = f"{str(n[0])} {('000 '*temp)} ".ljust(ljust_length)
        powers.append(f"{number}{units[count]}{s[1:]}")
        count += 1

    return powers

print("\n".join(power(n)))
```

## Tests
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz%2010%20%20tests.png)

## Flow Diagram
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz_010_FlowDiagram.jpeg)
