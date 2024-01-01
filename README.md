# Selection sort and Insertion sort
NAME : ALIYA SHEEMA
REFERENCE NUMBER : 23005529
DEPARTMENT : AIDS
## AIM :
To write a program to perform selection sort and insertion sort using python programming.
## EQUIPMENT'S REQUIRED :
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## ALGORITHM :
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
## PROGRAM :
i)	#Selection Sort
```
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: ALIYA SHEEMA
RegisterNumber: 23005529
'''
def selection_sort(nums):
    for i in range(len(nums)):
        lowest_value_index=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[lowest_value_index]:
                lowest_value_index=j
        nums[i],nums[lowest_value_index]=nums[lowest_value_index],nums[i]
list_of_nums=eval(input())
selection_sort((list_of_nums))
print(list_of_nums)

```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: ALIYA SHEEMA
RegisterNumber: 23005529
'''
def insertion_sort(nums):
    for i in range(1,len(nums)):
        item_to_insert=nums[i]
        j=i-1
        while j>=0 and nums[j]>item_to_insert:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=item_to_insert
list_of_nums=eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)

```

## OUTPUT :
i)	#Selection Sort

![selection_sort](https://github.com/23005529/Sorting-Algorithm/assets/139842207/928aed9b-3516-4436-81c0-042cb23092b7)

ii)	#Insertion Sort

![Insertion_sort](https://github.com/23005529/Sorting-Algorithm/assets/139842207/44732d57-a6ce-4c5c-ada8-57229a2735ff)



## RESULT :
Thus the program is written to perform selection sort and insertion sort using python programming.
