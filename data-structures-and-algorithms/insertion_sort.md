# Insertion Sort Cheatsheet

## Overview

- Insertion sort is a simple sorting algorithm.
- It works by iterating through the array, comparing each element with the previous elements, and inserting it into its correct position.
- It is efficient for small data sets, but inefficient for large data sets.

## Algorithm

```python
def insertion_sort(arr):
    # Traverse through 1 to len(arr)
    for i in range(1, len(arr)):
        key = arr[i]
        j = i - 1
        # Move elements of arr[0..i-1], that are greater than key, to one position ahead of their current position
        while j >= 0 and key < arr[j]:
            arr[j + 1] = arr[j]
            j -= 1
        arr[j + 1] = key
```

## Time Complexity

- Worst-case performance: O(n^2)
- Best-case performance: O(n)
- Average-case performance: O(n^2)

## Resources

- [Insertion Sort Wikipedia](https://en.wikipedia.org/wiki/Insertion_sort)
- [GeeksforGeeks: Insertion Sort](https://www.geeksforgeeks.org/insertion-sort/)
- [Visualgo: Insertion Sort](https://visualgo.net/en/sorting)