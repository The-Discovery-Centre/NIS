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

# October 25th Solution



```python
myList = []

while True:
    action = input("choose an action\n\ta - create a record\n\tv - view all records\n\tq - quit \n\n\t action: ")
    print("")
    print("")
    if action == "q":
        break
    elif action == "a":
        name = input("Enter the name: ")
        math = input("Enter the score in math: ")
        english = input("Enter the score in english: ")
        swahili = input("Enter the score in swahili: ")
        physics = input("Enter the score in physics: ")
        
        myList.append([name, int(math), int(english), int(swahili), int(physics)])
    elif action == "v":
        print(myList)
    else:
        print("Invalid action")
```

    choose an action
    	a - create a record
    	v - view all records
    	q - quit 
    
    	 action: a
    
    
    Enter the name: Gift
    Enter the score in math: 2
    Enter the score in english: 3
    Enter the score in swahili: 4
    Enter the score in physics: 5
    choose an action
    	a - create a record
    	v - view all records
    	q - quit 
    
    	 action: a
    
    
    Enter the name: Ethos
    Enter the score in math: 1
    Enter the score in english: 3
    Enter the score in swahili: 5
    Enter the score in physics: 7
    choose an action
    	a - create a record
    	v - view all records
    	q - quit 
    
    	 action: v
    
    
    [['Gift', 2, 3, 4, 5], ['Ethos', 1, 3, 5, 7]]
    choose an action
    	a - create a record
    	v - view all records
    	q - quit 
    
    	 action: q
    
    


# Challenge

Make a program such that the output is: 

    Gift got 3 in math, 7 in english, 8 in kiswahili and 9 in physics. Total is 27
    .
    .
    .
    
    Thanos got 8 in math, 10 in english, 9 in kiswahili and 9 in physics. Total is 36
    
# Solution

We can get the solution from the previous assignment



```python
myList = []

while True:
    action = input("choose an action\n\ta - create a record\n\tv - view all records\n\tq - quit \n\n\t action: ")
    print("")
    print("")
    if action == "q":
        break
    elif action == "a":
        name = input("Enter the name: ")
        math = input("Enter the score in math: ")
        english = input("Enter the score in english: ")
        swahili = input("Enter the score in swahili: ")
        physics = input("Enter the score in physics: ")
        
        myList.append([name, int(math), int(english), int(swahili), int(physics)])
    elif action == "v":
        for item in myList:
            name = item[0]
            math = item[1]
            english = item[2]
            kiswahili = item[3]
            physics = item[4]

            # calculate total marks
            total = math + english + kiswahili + physics


            print("{} got {} in math, {} in english, {} in kiswahili and {} in physics. Total is {}".format(name,math,english,kiswahili,physics, total))
    else:
        print("Invalid action")
```

    choose an action
    	a - create a record
    	v - view all records
    	q - quit 
    
    	 action: a
    
    
    Enter the name: Gift
    Enter the score in math: 1
    Enter the score in english: 2
    Enter the score in swahili: 3
    Enter the score in physics: 4
    choose an action
    	a - create a record
    	v - view all records
    	q - quit 
    
    	 action: a
    
    
    Enter the name: Ethos
    Enter the score in math: 1
    Enter the score in english: 3
    Enter the score in swahili: 5
    Enter the score in physics: 7
    choose an action
    	a - create a record
    	v - view all records
    	q - quit 
    
    	 action: v
    
    
    Gift got 1 in math, 2 in english, 3 in kiswahili and 4 in physics. Total is 10
    Ethos got 1 in math, 3 in english, 5 in kiswahili and 7 in physics. Total is 16
    choose an action
    	a - create a record
    	v - view all records
    	q - quit 
    
    	 action: q
    
    



```python

```


### ???
