# Guessing game
## Solution
```.py
# Generating the random number
import random
num = random.randint(1, 100)

i = input("Your guess: ")

if i.isnumeric():
    i = int(i)
else:
    quit()
while i != num:
    if i>num:
        print("Your guess is higher than the number")
        i = input("Your guess: ")
        break
    else:
        print("Your guess is lower than the number")
        i = input("Your guess: ")
print("You guessed correctly")
```

## Tests
![](https://github.com/thumulakaru/Unit-1/blob/main/Coding%20exercise/Guessing%20game.png)
