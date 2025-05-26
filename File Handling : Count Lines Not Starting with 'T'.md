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
  with open('story.txt', 'w') as file:
      file.write("This is the first line.\n")
      file.write("Another line starts here.\n")
      file.write("That’s yet another line.\n")
      file.write("One more line not starting with T.\n")
  
  with open('story.txt', 'r') as file:
      count = 0  
      for line in file:
          if not line.lstrip().startswith('T'):
              count += 1  
  
  print("Number of lines that do not start with 'T':", count)
```

## Output
![image](https://github.com/user-attachments/assets/81b43b85-26c3-4e3d-93a5-eed99e5df921)


## Result
Thus,the program has been executed successfully.
