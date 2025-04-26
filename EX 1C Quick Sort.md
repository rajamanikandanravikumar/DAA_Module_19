# EX 1C Quick Sort
## DATE: 26-04-2025
## AIM:
To write a python program to implement quick sort using tha last element as pivot on the list of float values.

## Algorithm
1. Choose a pivot element usually the last element of the array.
2. Rearrange the array so that.All elements smaller than or equal to the pivot go to the left.All elements greater than the pivot go to the right.
3. Place the pivot element in its correct sorted position.
4. Recursively apply the same steps to the sub-arrays on the left and right of the pivot.
5.Stop when the sub-array has 1 or 0 elements already sorted. 

## Program:
```
/*
Program to implement implement quick sort using the last element as pivot on the list of float values.
Developed by: RAJAMANIKANDAN R
Register Number:  212223220082
*/
def partition(arr, low, high):
    pivot = arr[high]
    i = low - 1
    for j in range(low, high):
        if arr[j] <= pivot:
            i += 1
            arr[i], arr[j] = arr[j], arr[i]
    arr[i + 1], arr[high] = arr[high], arr[i + 1]
    return i + 1

def quickSort(arr, low, high):
    if low < high:
        pi = partition(arr, low, high)
        quickSort(arr, low, pi - 1)
        quickSort(arr, pi + 1, high)

n = int(input())
arr = [float(input()) for _ in range(n)]
print("Sorted array is:")
quickSort(arr,0,n-1)
for num in arr:
    print(num)
```

## Output:
![image](https://github.com/user-attachments/assets/fcd89df7-da7c-4b76-aad2-4950e3a49935)



## Result:
The program successfully sorts the input array using the QuickSort algorithm, arranging the elements in ascending order.
