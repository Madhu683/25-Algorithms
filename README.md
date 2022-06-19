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
