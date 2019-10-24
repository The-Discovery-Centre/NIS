# NIS
## Python for Kids
NIS Intermediate level python problems and Solutions for Kids. 

# October 4th Solution

## Dataset
    
    id | name    | math   | english | Kiswahili | Physics
    -----------------------------------------------------
    1. | Gift    |   3    |   7     |   8       |   9
    2. | Krishna |   10   |   8     |   8       |   10
    3. | Ethos   |   5    |   1     |   2       |   6
    4. | Thanos  |   8    |   10    |   9       |   9 



```python
myList = [
    ['Gift', 3, 7, 8, 9],
    ['Krishna', 10, 8, 8, 10],
    ['Ethos', 5, 1, 2, 6],
    ['Thanos', 8, 10, 9, 9]
]
```


```python
print(myList)
```

    [['Gift', 3, 7, 8, 9], ['Krishna', 10, 8, 8, 10], ['Ethos', 5, 1, 2, 6], ['Thanos', 8, 10, 9, 9]]


## Challenge

Make a program such that the output is: 

    Gift got 3 in math, 7 in english, 8 in kiswahili and 9 in physics. Total is 27
    .
    .
    .
    
    Thanos got 8 in math, 10 in english, 9 in kiswahili and 9 in physics. Total is 36
    
## Solution


```python
for item in myList:
    name = item[0]
    math = item[1]
    english = item[2]
    kiswahili = item[3]
    physics = item[4]
    
    # calculate total marks
    total = math + english + kiswahili + physics
    
    
    print("{} got {} in math, {} in english, {} in kiswahili and {} in physics. Total is {}".format(name,math,english,kiswahili,physics, total))
```

    Gift got 3 in math, 7 in english, 8 in kiswahili and 9 in physics. Total is 27
    Krishna got 10 in math, 8 in english, 8 in kiswahili and 10 in physics. Total is 36
    Ethos got 5 in math, 1 in english, 2 in kiswahili and 6 in physics. Total is 14
    Thanos got 8 in math, 10 in english, 9 in kiswahili and 9 in physics. Total is 36


### ???
