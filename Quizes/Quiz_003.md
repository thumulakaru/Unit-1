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
```.py
protein_in = input("Please enter the protein chain:")
protein_out = ("")
for letter in protein_in:
    if letter == "A":
        protein_out = (protein_out + "T")
    elif letter == "G":
        protein_out = (protein_out + "C")
    elif letter == "T":
        protein_out = (protein_out + "A")
    elif letter == "C":
        protein_out = (protein_out + "G")
    else:
        print("Error")
print("Answer to the protein that you inputted is " + protein_out + ".")
```

## Tests
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-09-04%20at%2010.15.01.png)

## Flow diagram
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz_003_FlowDiagram.jpg)
