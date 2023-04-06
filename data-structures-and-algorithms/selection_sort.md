# Selection Sort Cheatsheet

## Overview

- Selection sort is a simple sorting algorithm.
- It works by repeatedly finding the minimum element from the unsorted part of the array and putting it at the beginning.
- It has O(n^2) time complexity, making it inefficient on large lists.

## Algorithm

```python
def selection_sort(arr):
    # Traverse through all array elements
    for i in range(len(arr)):
        # Find the minimum element in remaining unsorted array
        min_index = i
        for j in range(i + 1, len(arr)):
            if arr[min_index] > arr[j]:
                min_index = j

        # Swap the found minimum element with the first element
        arr[i], arr[min_index] = arr[min_index], arr[i]
```

## Time Complexity

- Worst-case performance: O(n^2)
- Best-case performance: O(n^2)
- Average-case performance: O(n^2)

## Resources

- [Selection Sort Wikipedia](https://en.wikipedia.org/wiki/Selection_sort)
- [GeeksforGeeks: Selection Sort](https://www.geeksforgeeks.org/selection-sort/)
- [Visualgo: Selection Sort](https://visualgo.net/en/sorting)