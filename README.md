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
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: ARUNMOZHI VARMAN T
RegisterNumber: 23002304

def selection_sort(nums):
    for i in range (len(nums)):
        low_index=i
        for j in range(i+1,len(nums)):
            if nums[j] < nums[low_index]:
                low_index=j
        nums[i],nums[low_index]=nums[low_index],nums[i]
    return nums    
    
list_of_nums = eval(input())
value = selection_sort(list_of_nums)
print(value)

```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: ARUNMOZHI VARMAN T
RegisterNumber: 23002304
'''
def insertion_sort(nums):
    for i in range (1, len(nums)):
        item_to_insert = nums[i]
        j = i - 1
        while j >= 0 and nums[j] > item_to_insert:
            nums[j+1] = nums[j]
            j -= 1
        nums[j+1] = item_to_insert
    
list_of_nums = eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)

```

## Output:
## selection sort
![Screenshot 2024-01-03 121108](https://github.com/etjabajasphin/Sorting-Algorithm/assets/144870523/10c9faf2-f4cc-479e-8098-87d9a49e75f2)

## insertion sort
![Screenshot 2024-01-03 121132](https://github.com/etjabajasphin/Sorting-Algorithm/assets/144870523/8baa4b85-4976-4c9c-a9a8-8208a3f8d075)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
