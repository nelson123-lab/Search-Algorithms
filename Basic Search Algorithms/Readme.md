The basic Search algorithms includes:

1) Linear search
   - Linear search is a simple search algorithm that iterates through a list of elements until it finds the desired value or reaches the end of the list.
   - Here, for a search query the iteration happens til n time. The time complexity of this operation is O(n)

### Linear Search python code
```python
def linear_search(listA, search_element):
  for idx, ele in enumerate(listA):
    if ele == search_element:
      return idx
    else: pass
  return "Elemnet Not Found"
```

2) Binary Search
   - Binary search is a search algorithm that efficiently works for a sorted list or array which uses a divide-and-conquer approach by repeatedly dividing the search space in half until the target value is found or absent.
   - The time complexity of the binary search algorithm is O(logn) for a sorted array and O(nlogn) for an unsorted array which takes into account of the sorting time complexity as well.

### Binary Search python code
```python
# Binary search by default assumes array as sorted.
def binary_search(listA, search_element):
  left, right = 0, len(listA)-1
  while left <= right:
    mid = (right+left)//2

    if listA[mid] == search_element:
      return mid
    elif listA[mid] > search_element:
      right = mid -1
    else:
      left = mid + 1
  return "Elemnet Not Found"
```
