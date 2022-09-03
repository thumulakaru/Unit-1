# Quiz 003
## solution to the SL problem
```.py
count = 0
while count != 4:
    in_protein = str(input("Please enter the protein:"))
    a = in_protein.upper()
    if a == "A":
        print("T")
        count = count+1
    elif a == "G":
        print("C")
        count = count + 1
    elif a == "T":
        print("A")
        count = count + 1
    elif a == "C":
        print("G")
        count = count + 1
    else:
        print("Error")
        count = 4
```
## Tests
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-09-03%20at%2015.10.31.png)

## Solution to the HL problem
Work in progress
