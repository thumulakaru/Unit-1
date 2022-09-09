# Median
## Solution
```.py
# Creating a list and getting the length of the data
data = []
num = int(input("Please enter the number of scores that you want to enter: "))

# Checking for invalid input
if num != 4 and num != 5:
    exit()

# Getting data from the user
for i in range(0, num):
    data.append(int(input("Input a number: ")))


# Making the list in the ascending order
data.sort()
if len(data) == 5:
    print(data[2])
elif len(data) == 4:
    print(int((data[1]+data[2])/2))
else:
    print("Invalid input")
```

## Tests
![](https://github.com/thumulakaru/Unit-1/blob/main/Coding%20exercise/Median%20tests-1.png)

**Figure 1:** Tests part 1

![](https://github.com/thumulakaru/Unit-1/blob/main/Coding%20exercise/Median%20tests-2.png)

**Figure 2:** Tests part 2 
