# Quiz 009
## Solution
```.py
def quiz_009(word_in:str , shift:int)->str:
# Naming the output
    word_out = ""
    for i in word_in:
        temp = ord(i)+shift
        temp = int(temp)
        if temp > 122:
            word_out += (chr(temp-26))
        else:
            if temp < 97:
                word_out += (chr(temp+26))
            else:
                word_out += (chr(temp))
    return word_out
word_in = input("Please enter a word:")
shift= int(input("Please enter the shift:"))

print(quiz_009(word_in, shift))

```

## Evidence
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz%209%20tests.png)

## Flowchart
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz_009_FlowDiagram.jpg)
