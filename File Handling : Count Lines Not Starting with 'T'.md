# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program
```
from collections import defaultdict


def create_file(file_path, content):
    with open(file_path, 'w') as file:
        file.write(content)

# Function to calculate character frequencies
def char_frequency(file_path):
    frequencies=defaultdict(int)
    with open(file_path,'r')as file:
        content=file.read()
        for char in content:
            frequencies[char]+=1
    return frequencies

```

## Output

<img width="950" height="413" alt="image" src="https://github.com/user-attachments/assets/a6924c67-8c00-4a0f-9c32-f8a8ff566991" />

## Result
The program is executed
