# Task 1: Computational thinking

## Research Questions
### Question 1
How a computer is able to predict what would happen to a nuclear weapon in another 50 years just using probability when the next moment of a human's life is still a question.

### Question 2
Developing supercomputers would help solve many problems in healthcare and also in many other fields. The Flash TV series is a perfect example for this. Even though the machine that is developed is not a supercomputer it can be seen as a symbol. But as the show itself proves that the machine brought harm to humanity likewise a supercomputer would also bring harm by developing new weaponary systems which would ultimately cause in a war due to getting the most technological advanced military equipment. In my opinion supercomputers should be developed but it also should be 100% transparent to civilians.

### Question 3
Since there are no details about super computers in Sri Lankan I will be using the Japan's highest speed supercomputer as the my home country's fastest computer. Japan's fastest supercomputer is 'supercomputer Fugaku'. It is mainly used for scientific researchs. It has 158,976 nodes. Which brings the fact that it is able to cool itself for sustained performances.

“Specification of Supercomputer Fugaku.” Supercomputer Fugaku : Fujitsu Global, https://www.fujitsu.com/global/about/innovation/fugaku/specifications/. 

## Programming Task
### Task 1
```.py
# Printing colours for 2400 lockers

# Defining colours
colours = ["blue", "red", "white", "yellow"]

# Defining the max number of locker
finallocker = 2400

# Printing the locker colour
for lockernum in range(1, finallocker+1):
# Getting the module to calculate the locker colour.
    lockermod = lockernum % 4
    print(f"For locker number {lockernum} the colour is {colours[lockermod]}." )
```

### Task 2
```.py
# Printing an output based on the locker number given by the user

# Get the input from the user
lockernum = int(input("Please enter the locker number:"))

# Defining the colours
colours = ["blue", "red", "white", "yellow"]

# Finding which colour is the input
lockermod = lockernum % 4
a = colours[lockermod]

# Output the number
print("For locker number " + str(lockernum) +" colour is " + a + ".")
```

### Task 3

```.py
# Printing an output based on the locker number given by the user


# Get the colour from the user
colour_in = input("Please enter the colour:")
colour_in = colour_in.lstrip()
colour_in = colour_in.rstrip()
locker = ""
# Checking the validity of the input
if not colour_in.isnumeric() and colour_in.isprintable():
    colour_in = colour_in.lower()
    colour_in = colour_in.capitalize()
    if colour_in == "Blue":
        for lock_num in range(1, 2401):
            lock_mod = lock_num % 4
            if lock_mod == 0:
                locker = locker + ", "+(str(lock_num))
    if colour_in == "Red":
        for lock_num in range(1, 2401):
            lock_mod = lock_num % 4
            if lock_mod == 1:
                locker = locker + ", "+(str(lock_num))
    if colour_in == "White":
        for lock_num in range(1, 2401):
            lock_mod = lock_num % 4
            if lock_mod == 2:
                lock_num = str(lock_num)
                locker = locker + ", "+(str(lock_num))
    if colour_in == "Yellow":
        for lock_num in range(1, 2401):
            lock_mod = lock_num % 4
            if lock_mod == 3:
                locker = locker + ", "+(str(lock_num))
else:
    colour_in = input("You entered a wrong input. Please enter a valid input")

print(f"You entered {colour_in.center(25)}.")
print(f"You will have the following lockers in {colour_in} "
      f"{locker}")
```

![](https://github.com/thumulakaru/Unit-1/blob/main/Tasks/Task%201.3%20Tests.png)

**Figure 1:** Tests for Task 1.3

### Task 4

```.py
import random

## Dictionary for names
names = dict()
names["Puhalskis"] = "Ralfs"
names["Karunaratne"] = "Thumula"
names["Chuao"] = "Jason"

last_name = ['Puhalskis', 'Karunaratne', 'Chuao']
with open('studentdirectory.txt', 'w') as file:
    pass

# Saving the data
for ln in last_name:
    templockernum = random.randint(1,2400)
    final = (f"{ln}, {names[ln]}, {names[ln]}.{ln}@uwcisak.jp, locker {templockernum}"),
    with open('studentdirectory.txt', 'a') as file:
        file.write(str(final))
        file.write("\n")
        file.close()
```
