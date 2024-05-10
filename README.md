# Linear Search and Binary search
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
#DEVELOPED BY : Vidhiya lakshmi S
#REG NO:212223230238
#Use a linear search method to match the item in a list.
def linearsearch(array, n, k):
    for i in range(0, n):
        if (array[i] == k):
            return i
    return -1
    
array= eval(input())
k= eval(input())
n= len(array)
array.sort()
result= linearsearch(array, n, k)
if (result== -1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ", result)


```
ii)	# Find the element in a list using Binary Search(Iterative Method).

```

#DEVELOPED BY : Vidhiya lakshmi S
#REG NO:212223230238
def binarySearchIter(lst, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if lst[mid]==k:
            return mid
        elif lst[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
lst = eval(input())
lst.sort()
k = eval(input()) 
print(lst)
res=binarySearchIter(lst,k,0,len(lst)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)

```
iii)	# Find the element in a list using Binary Search (recursive Method).

```
#DEVELOPED BY : Vidhiya lakshmi S
#REG NO:212223230238
def binarySearchIter(lst, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if lst[mid]==k:
            return mid
        elif lst[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
lst = eval(input())
lst.sort()
k = eval(input()) 
print(lst)
res=binarySearchIter(lst,k,0,len(lst)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)

```
## Sample Input and Output

![Screenshot 2024-05-10 152720](https://github.com/saravidhya/Search-Algorithms/assets/87062069/ed9de4e7-46fe-4fcb-8c76-d5e85f8746bb)


![Screenshot 2024-05-10 152734](https://github.com/saravidhya/Search-Algorithms/assets/87062069/eab4d3ca-b606-4a22-966a-4427caa4edbb)


![Screenshot 2024-05-10 152753](https://github.com/saravidhya/Search-Algorithms/assets/87062069/20f917e2-dd7b-40ca-9cf1-985e3a2b4088)



## Result
Thus the linear search and binary search algorithm is implemented using python programming.
