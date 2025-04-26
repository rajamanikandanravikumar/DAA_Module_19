# EX 1D Linear search
## DATE: 26-04-2025
## AIM:
To write a python program for a search function with parameter list name and the value to be searched using string values.



## Algorithm
1. Start from the first element of the array.
2. Compare the target value with the current element.
3. If they match, return the index or say "Element found" and if not, move to the next element.
4. Repeat until the end of the array.
5. If the element is not found after checking all, say "Element not found". 

## Program:
```
/*
Program to implement a search function with parameter list name and the value to be searched using string values.
Developed by: RAJAMANIKANDAN R
Register Number:  212223220082
*/
def search(List,n):
    
    found = False
    for ele in List:
        if ele == n :
            found = True
            break
    if found :
        print("Found")
    else:
        print("Not Found")

l = int(input())
List = [str(input()) for _ in range(l)]
n = str(input())

```

## Output:
![image](https://github.com/user-attachments/assets/8b3e4549-ab28-4dcb-9d44-3969694ef432)

## Result:
The program was executed successfully, and it correctly checks if the input element is present in the list, printing "Found" if the element exists or "Not Found" if it does not.
