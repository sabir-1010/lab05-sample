# lab05-sample
# Sample_solution_W23

## Sample Solution: TASK2 (PartA without built-in function to find element)
 
```python
def finding_Func(myList, myCheckNum):
    for i in range(len(myList)):
        #using for-loop to go through all the element, NOT built-in function to find element
        if list[i] == myCheckNum:
            print("The element is found at index", i)
            return
    print("The element does not exist in the list")

##this is the test case part. main code is above this finding_Func function 
list = [2, 4, 6, 8, 10, 12, 14, 16]
number = 4
index = finding_Func(list, number)
```
The output will look like: `The element is found at index 1`


## Sample Solution: TASK2 (PartB using built-in function to find element)
 
```python
def finding_Func(myList, myCheckNum):
    #using a built-in function 'in' to find element. It doesnt not require the for-loop like part A. 
    #Direclty tell me whether the element exist or not. 
    # used "list.index(number)" to find the index location
    if myCheckNum in myList:
        print("The element is found at index", list.index(number))
    else:
        print("The element does not exist in the list")

#this is the test case part. main code is above this finding_Func function
list = [2, 4, 6, 8, 10, 12, 14, 16]
number = 29
index = finding_Func(list, number)
```
The output will look like: `The element does not exist in the list`


## Sample Solution: TASK1 (print out multiples of 3 between 0 and 100 which are divisible by 2)
 
```python
for x in range(0,101,3):
    if x%2==0:
        print(x)
```
The output will look like: `0
6
12
18
24
30
36
42
48
54
60
66
72
78
84
90
96`
