# Task 1(13.09.2022)

## Task 1
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

## Task 2
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

## Task 3

