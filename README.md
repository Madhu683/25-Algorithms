# 25-Algorithms
## 1. Linear Search
**Linear Search algorithm is also known as sequential search. It search an element in array by visting elements sequentialy or linearly. It is basic approach to search an element in an array.**
```python
## arr--->Array
## x  ---> searching element
LinearSearch(arr,x):
     for(i=0;i<arr.len();i++):
           if x==arr[i]:
               return i     ## return index of element in array
     return -1              ## return -1 if element is not found in array
           
```
![linear_search](https://user-images.githubusercontent.com/70106840/174482112-02654a55-688d-4014-b0cd-e4b78d967cb7.gif)

**Time complexity:O(n)**

**Space complexity:O(1)**
## 2. Binary Search
**Binary Search is effcient than Linear Search. It sorts the array after that it searches the element in array by repeatedly dividing search interval in half.**

![binary_search](https://user-images.githubusercontent.com/70106840/174483072-603fd364-8764-4e97-979e-012af418d09e.gif)

### Iterative approach
```python
##arr ---> Array
##low ---> lower index of an array
##high -->Higher index of an array
##x   ---> searching element
BinarySearch(arr,low,high,x):
      sort(arr)                    ## sort the array
      while(low<high):
            mid = (low+high)/2
            if x==arr[mid]:
                return mid        ## if element found return the index of element in array
            else if(x>arr[mid]): 
                low=mid+1         ## if element is greater than mid index element shift the low to mid+1
            else 
                high=mid-1        ## if element is lower than mid index element sift the high to mid-1
      return -1                   ## return -1 if element not found in array
          
```
