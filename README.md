# Linear Search and Binary search
NAME: DEVA DHARSHINI I

REGISTER NUMBER: 212223240026

DEPARTMENT: AIML

## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
Program to  perform linear search and binary search using python programming.
Developed by : DEVA DHARSHINI I
RegisterNumber : 212223240026
def linearSearch(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
print(array)
res=linearSearch(array,k,0,len(array)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)
```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
Program to  perform linear search and binary search using python programming.
Developed by : DEVA DHARSHINI I
RegisterNumber : 212223240026
def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
print(array)
res=binarySearchIter(array,k,0,len(array)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)
```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
Program to  perform linear search and binary search using python programming.
Developed by : DEVA DHARSHINI I
RegisterNumber : 212223240026
def binarySearchrec(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
print(array)
res=binarySearchrec(array,k,0,len(array)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)

```
## Sample Input and Output
i)	#Use a linear search method to match the item in a list.
![Screenshot 2024-04-16 202151](https://github.com/deesk13/Search-Algorithms/assets/150927063/ea3d5c31-1bb6-427e-bab4-be0b13ceefa6)
ii)	# Find the element in a list using Binary Search(Iterative Method).
![Screenshot 2024-04-16 202207](https://github.com/deesk13/Search-Algorithms/assets/150927063/b805ca54-ac84-47bb-86e6-19bdca5cecc2)
iii)	# Find the element in a list using Binary Search (recursive Method).
![Screenshot 2024-04-16 202228](https://github.com/deesk13/Search-Algorithms/assets/150927063/2e243966-fd7a-4fe4-bf0d-f9ac7a2f4890)


## Result
Thus the linear search and binary search algorithm is implemented using python programming.
