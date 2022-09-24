# Quiz 011

## Solution
```.py
# Defining month's days
jan_oct_days = ["Sa", "Su", "Mo", "Tu", "We", "Th", "Fr"]
feb_sep_nov_days = ["Tu", "We", "Th", "Fr", "Sa", "Su" ,"Mo"]
apr_may_jul_days = ["Fr", "Sa", "Su", "Mo", "Tu", "We", "Th"]
mar_days = ["Su", "Mo", "Tu", "We", "Th", "Fr", "Sa"]
jun_days = ["We", "Th", "Fr", "Sa", "Su", "Mo", "Tu"]
aug_days = ["Mo", "Tu", "We", "Th", "Fr", "Sa", "Su"]
dec_days = ["Th", "Fr", "Sa", "Su", "Mo", "Tu", "We"]

# Get the input from user
month_in = input("Please enter the month:")
month_in = month_in.lower()

# Defining the function
def best_month(month_in:str):
    out = ""
    # Defining the list for the relevant month
    if month_in == "jan" or month_in == "oct":
        current_month_days = jan_oct_days
    elif month_in in ["feb","sep","nov","dec"]:
        current_month_days = feb_sep_nov_days
    elif month_in in ["may",  "apr", "jul"]:
        current_month_days = apr_may_jul_days
    elif month_in in "mar":
        current_month_days = mar_days
    elif month_in in "jun":
        current_month_days = jun_days
    elif month_in in "aug":
        current_month_days = aug_days
    elif month_in in "dec":
        current_month_days = dec_days
    else:
        print("Wrong input")
    for b in range(1, 32):
        i = b-1
        out += str(current_month_days[i % 7]) + " " + str(b) + "\n"
    return out

print(best_month(month_in))
```

## Tests
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz%2010%20%20tests.png)


## Flow Diagram
### Part 1
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz_011_FlowDiagram_part1.png)

### Part 2
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz_011_FlowDiagram_part2.png)
