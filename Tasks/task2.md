# Task 2
This task was designed as an example for reading a file via python

## Solution
```.py
# Example program for writing and reading files in python
def validate_int_input(prompt:str)->int:
    '''this function asks the user for an input
    and validates that the input is an integer
    returns:integer'''
    end_code = "\033[00m"
    red = "\033[0;33m"
    num = input(prompt)
    while not num.isdigit():
        num = input(f"{red}Error {prompt}{end_code}")

    return int(num)


colours = ["\033{0;30m", "\033[0;31m", "\033[0;32m", "\033[0;34m"]
end_code = "\033[0;30m"

intro_msg = f"{colours[1]} Welcome to EV calculator{end_code}"
print(intro_msg.center(50, "-"))

menu = """1. Average time per kWh\n
2. Total kWh used\n
3. Total all data\n
4. Show all data
"""

print("Options".center(50))
print(menu)

option = validate_int_input("Please enter an option [1-4]: ")
while option > 4 or option < 1:
    option = validate_int_input(f"{option} is incorrect. Please enter an option [1-4]")

# This is how to read a file
with open("charging_log.csv", "r") as file:
    ev_data = file.readlines()
# Solve option 1
if option == 1:
    i = 0
    total_use = 0
    for line in ev_data:
        if i > 0:
            values = line.split()
            use_time = values[2]
            hms = use_time.split(":")
            hours = int(hms[0]) * 3600
            minutes = int(hms[1]) * 60
            seconds = int(hms[2])
            total_use = total_use + hours + minutes + seconds
        i += 1
    i = 0
    total_charge = 0
    for line in ev_data:
        if i > 0:  # This skips the first line
            values = line.split()
            charge = values[1]
            charge_clean = charge[:5]  # Without the unit
            charge_float = float(charge_clean)
            total_charge += charge_float
        i += 1
    average_in_seconds = total_use / total_charge
    final_hours = int(average_in_seconds//3600)
    final_minutes = int((average_in_seconds%3600)//60)
    final_seconds = int(((average_in_seconds%3600)%60))
    print(f"The average time per kWh is {final_hours}:{final_minutes}:{final_seconds}.")

# Solve option 2
if option == 2:
    i = 0
    total_charge = 0
    for line in ev_data:
        if i > 0: # This skips the first line
            values = line.split()
            charge = values[1]
            charge_clean = charge[:5]#Without the unit
            charge_float = float(charge_clean)
            total_charge += charge_float
        i += 1
    print(total_charge)

# Solve option 3
if option == 3:
# Total charge
    i = 0
    total_charge = 0
    for line in ev_data:
        if i > 0:  # This skips the first line
            values = line.split()
            charge = values[1]
            charge_clean = charge[:5]  # Without the unit
            charge_float = float(charge_clean)
            total_charge += charge_float
        i += 1
    i = 0
    total_use = 0
    for line in ev_data:
        if i > 0:
            values = line.split()
            use_time = values[2]
            hms = use_time.split(":")
            hours = int(hms[0]) * 3600
            minutes = int(hms[1]) * 60
            seconds = int(hms[2])
            total_use = total_use + hours + minutes + seconds
        i += 1
    final_hours = int(total_use // 3600)
    final_minutes = int((total_use % 3600) // 60)
    final_seconds = int(((total_use % 3600) % 60))
    print(f"The total used electricity is {total_charge}kWh.")
    print(f"The total time used for electricity is {final_hours}:{final_minutes}:{final_seconds}.")


# Solve option 4
if option == 4:
    i = 0
    for line in ev_data:
        #strip removes the /n from the string
         if i > 0:
            line = line.strip()
            print(f"{colours[3]}Log No.{i}{line}{end_code}")
         i += 1
```
## Tests

### Option 1
![](https://github.com/thumulakaru/Unit-1/blob/main/Tasks/Task%202%20Test%201.png)

### Option 2
![](https://github.com/thumulakaru/Unit-1/blob/main/Tasks/Task%202%20Test%202.png)

## Option 3
![](https://github.com/thumulakaru/Unit-1/blob/main/Tasks/Task%202%20Test%203.png)

## Option 4
![](https://github.com/thumulakaru/Unit-1/blob/main/Tasks/Task%202%20Test%204.png)
