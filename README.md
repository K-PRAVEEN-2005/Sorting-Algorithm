# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by:PRAVEEN K
RegisterNumber:23014148 
'''
def selection_sort(nums):
    n= len(nums)
    for i in range(n-1):
        min_index = i
        for j in range(i+1,n):
            if nums[j] < nums[min_index]:
                min_index = j
        nums[i], nums[min_index]= nums[min_index], nums[i]
    return nums
list_of_nums = eval(input())
sorted_list = selection_sort(list_of_nums)
print(sorted_list)
        
 





```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by:PRAVEEN K
RegisterNumber:23014148 
'''
def insertion_sort(arr):
    n= len(arr)
    if n<=1:
        return
    for i in range(1,n):
        key=arr[i]
        j=i-1
        while j>=0 and key<arr[j]:
            arr[j+1]=arr[j]
            j-=1
        arr[j+1]=key
arr = eval(input())
insertion_sort(arr)
print(arr)
            
         
 
        
 





```

## Output:
 ![Alt text](<python 4 th1.png>)
  ![Alt text](<python 4 th 2.png>) 

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
