# CSE 15L (Third Lab report)

In this lab, I am going to be reporting my findings on research on the grep command. There are 4 possible variations of the grep command: 

* grep "some string" <name of .txt file>
  
* grep -v <name of .txt file>
  
* grep -n <name of .txt file>
  
* grep -c <name of .txt file>
  
  
## First type
### grep "some string" <name of .txt file>
  
  
This type of grep gives an output which shows all lines that have "some string" word in the line. Below are two examples.
  
  ```
# First code block example
grep "WhatToDo" find-results.txt
```
  
This is the output you receive when trying to find the number of lines which have "WhatToDo" in the find-results.txt file.
  
![First Output](Report3ImageOne.jpg)

  
  ```
# code block
grep "History" find-results.txt
```
