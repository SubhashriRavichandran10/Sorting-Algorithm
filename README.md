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
Developed by:R.Subhashri
RegisterNumber:23012776
'''
def selection_sort(nums):
    for i in range(len(nums)):
        lowest_value_index = i
        for j in range(i+1 , len(nums)):
            if nums[j] < nums[lowest_value_index]:
                lowest_value_index = j
        nums[i], nums[lowest_value_index] = nums[lowest_value_index], nums[i]
        
list_of_nums = eval(input())
selection_sort(list_of_nums)
print(list_of_nums)
    




```
ii)	#Insertion Sort
```

Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by:R.Subhashri
RegisterNumber:23012776 
'''
def insertion_sort(arr):
    for i in range(1,len(arr)):
        a=arr[i]
        j=i-1
        
        while j>=0 and a<arr[j]:
            arr[j+1]=arr[j]
            j-=1
        arr[j+1]=a
    return arr
    
arr= eval(input())
print(insertion_sort(arr))








```

## Output:

![Screenshot 2024-01-02 133349](https://github.com/SubhashriRavichandran10/Sorting-Algorithm/assets/145743413/6a6e6aea-417d-4f2c-b1ad-7812569558d4)

![Screenshot 2024-01-02 133407](https://github.com/SubhashriRavichandran10/Sorting-Algorithm/assets/145743413/63bb4465-1c50-4f5f-89d8-bc69bfb5cb46)




## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
