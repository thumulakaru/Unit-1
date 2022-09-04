# Coding Exercise - Salary
## Solution
```.py
salary = int(input("Please enter the salary:"))
if salary > 10001:
    if salary > 50001:
        if salary > 100001:
            print("Your tax for the salary entered is "+str(salary*25/100)+" USD")
        else:
            print("Your tax for the salary entered is " + str(salary*15/100)+" USD")
    else:
        print(str(salary*10/100))
elif salary>0 and salary :
    print("Your tax for the salary entered is "+str(salary*5/100)+ " USD")
else:
    print("You entered a wrong value")
```

## Test
![](https://github.com/thumulakaru/Unit-1/blob/main/Screen%20Shot%202022-09-04%20at%2011.07.45.png)
