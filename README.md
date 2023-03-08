# lab05-sample
# Sample_solution_W23

## Sample Solution: TASK2 (PartA without built-in function to find element)
 
```python
def finder(list, number):
    for i in range(len(list)):
        if list[i] == number:
            print("The element is found at index", i)
            return
    print("The element does not exist in the list")
list = [2, 4, 6, 8, 10, 12, 14, 16]
number = 29
index = finder(list, number)
```


## Sample Solution: TASK2 (PartB using built-in function to find element)
 
```python
def finder(list, number):
    if number in list:
        print("The element is found at index", list.index(number))
    else:
        print("The element does not exist in the list")
list = [2, 4, 6, 8, 10, 12, 14, 16]
number = 2
index = finder(list, number)
```
