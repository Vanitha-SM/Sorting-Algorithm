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
Program for linear search method to match the item in a list
Developed by: Vanitha S
RegisterNumber: 212222100057
'''
def linearSearch(array,n,k):
    for i in range(0,n):
        if(array[i]==k):
            return i
    return -1
    
array = eval(input())
# sort the array
k = eval(input()) # k-item to be seared for
n=len(array)# get the length of array and store in the variable n
array.sort()
result = linearSearch(array,n,k)# use the function for linear search
print(array)
if(result==-1):
    print("Element not found")
else:
    print("Element found at index: ",result)     
# use if-else to print sorted array and "Element not found" if the item is not present in the list otherwise print sorted array and "Element found at index: ", result


```
ii)	#Insertion Sort
```
''' 
Program to find the element in a list using Binary Search(Iterative Method)..
Developed by: Vanitha S
RegisterNumber: 212222100057
'''
def binarySearchIter(array, k, low, high):
    mid=0
    while low<=high:
        mid=(high+low)//2
        if(array[mid]<k):
            low=mid+1
        elif(array[mid]>k):
            high=mid-1
        else:
            return mid
    return -1

array = eval(input())
array.sort()# sort the array
k = eval(input()) #k-item to be searched
res=binarySearchIter(array, k, 0,len(array)-1)
# use the binary search function to find the item in the list
print(array)
if(res==-1):
    print("Element not found")
else:
    print("Element found at index: ",res)
# use if-else to print sorted array and "Element not found" if the item is not present in the list otherwise print sorted array and "Element found at index: ", result

```

## Output:
![output](/Sorting-Algorithm/img/3b1.png)


![output](/Sorting-Algorithm/img/3b2.png)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
