# Bubble Sort Cheatsheet

## Overview

- Bubble sort is a simple sorting algorithm.
- It works by repeatedly swapping adjacent elements if they are in the wrong order.
- Each pass through the array places the next largest value in its proper place.

## Algorithm

```python
def bubble_sort(arr):
    n = len(arr)

    # Traverse through all array elements
    for i in range(n):
        # Last i elements are already in place
        for j in range(0, n - i - 1):
            # Swap if the element found is greater than the next element
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]
```

## Time Complexity

- Worst-case performance: O(n^2)
- Best-case performance: O(n)
- Average-case performance: O(n^2)

## Resources

- [Bubble Sort Wikipedia](https://en.wikipedia.org/wiki/Bubble_sort)
- [GeeksforGeeks: Bubble Sort](https://www.geeksforgeeks.org/bubble-sort/)
- [Visualgo: Bubble Sort](https://visualgo.net/en/sorting)