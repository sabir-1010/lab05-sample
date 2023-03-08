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
    #using a built-in function 'in' to find element. It doesnt not require the for-loop like part A
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
