# Quiz 16
## Solution
```.py
def blackboxthree(prompt:str) -> str:
    letter_list = []
    prompt = prompt.lower()
    for letter in prompt:
        letter_list.append(letter)
    n = -1

    out = ""
    for element in letter_list:
        count = 1
        n += 1
        for i in range(0, n):
            if element == letter_list[i] and element != " ":
                count += 1
            elif element == " ":
                out += " "
                count = ""
                break
        out += str(count)
    return out


user_in = input("Please enter your choice:")
print(blackboxthree(user_in))
```

## Tests
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz%2016%20tests%20part.1.png)

![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz%2016%20tests%20part.2.png)

![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz%2016%20tests%20part.3.png)

![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz%2016%20tests%20part.4.png)

## Flow diagrams
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz_016_FlowDiagram.png)
