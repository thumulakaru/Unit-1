# Solution to quiz_001

![](https://github.com/thumulakaru/Unit-1/blob/main/Quiz_001.jpg)

**Fig. 1** This is the solution to the black box

**Fig. 1** Shows my solution to the quiz001. The procedure to generate the outputs below are


| Input                       | Output          |
|-----------------------------|-----------------|
|        international        |       i11l      |
| (Cats) + (Dogs) = (Trouble) | (4) + (4) = (8) |
|                             |                 |

# My BlackBox

When the user enters a word the program outputs the first letter, number of characters in between the first two letters and the last letter.

## Solution
```.py
word_in = input("Please enter a word:")
word_len = len(word_in)

if word_len > 2:
    out = word_in[0] + str(word_len-2) + word_in[word_len-1]
else:
    out = word_in

print(out)
```

## Tests
![](https://github.com/thumulakaru/Unit-1/blob/main/Quizes/Quiz%201%20tests.png)
