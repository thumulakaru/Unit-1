# Quiz 007 

## SL problem
```.py
import random


for x in range(1, 11):
    out = ""
    for i in range(1, 21):
        rand_ascii = random.randint(48, 122)

        while 57 < rand_ascii < 65 or 90 < rand_ascii < 97:
            rand_ascii = random.randint(48, 122)
        else:
            out = out + str(chr(rand_ascii))
    print(out)
```


![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz%207%20tests(SL).png)

**Figure 1:** Tests for SL

## HL problem
```.py
import random
length = int(input("Please enter the length of the password:"))
symbols = input("Do you want symbols in the password? Please answer \"yes\" or \"no\":")

validity = False
while validity != False:
    symbols.lower()
    if symbols == "yes" or symbols == "no":
        validity = True
    else:
        symbols = input("Wrong input. Please enter \"yes\" or \"no\":")

if symbols == "yes":
    char = True
elif symbols == "no":
    char = False

if char == False:
    for x in range(1, 11):
        out = ""
        for i in range(1, 21):
            rand_ascii = random.randint(48, 122)

            while 57 < rand_ascii < 65 or 90 < rand_ascii < 97:
                rand_ascii = random.randint(48, 122)
            else:
                out = out + str(chr(rand_ascii))
        print(out)
elif char == True:
    for x in range(1, 11):
        out = ""
        for i in range(1, length + 1):
            rand_ascii = random.randint(33, 126)

            while not(33< rand_ascii < 126):
                rand_ascii = random.randint(33, 126)
            else:
                out = out + str(chr(rand_ascii))
        print(out)
```

![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz%207%20tests(HL).png)

**Figure 2:** Tests for HL

