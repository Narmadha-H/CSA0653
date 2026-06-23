# Debugging Selection Sort (Incorrect Minimum Index Update)

## Problem Statement
The given Selection Sort program does not correctly sort the array because of an error in updating the minimum index.

## Given Code

```python
def selection_sort(arr):
    n = len(arr)
    for i in range(n):
        min_idx = i
        for j in range(i+1, n):
            if arr[j] < arr[min_idx]:
                min_idx = i      # ERROR
        arr[i], arr[min_idx] = arr[min_idx], arr[i]
    return arr
```

## Error Identification
The statement

```python
min_idx = i
```

is incorrect.

It should be:

```python
min_idx = j
```

because when a smaller element is found, its index (`j`) should be stored.

## Effect of the Error
- The algorithm never updates the position of the minimum element.
- The correct minimum element is not selected.
- The array remains unsorted or partially sorted.

## Corrected Program

```python
def selection_sort(arr):
    n = len(arr)

    for i in range(n):
        min_idx = i

        for j in range(i + 1, n):
            if arr[j] < arr[min_idx]:
                min_idx = j

        arr[i], arr[min_idx] = arr[min_idx], arr[i]

    return arr


arr = [64, 25, 12, 22, 11]
print("Sorted Array:", selection_sort(arr))
```

## Output

```text
Sorted Array: [11, 12, 22, 25, 64]
```

## Time Complexity

| Case | Complexity |
|------|------------|
| Best Case | O(n²) |
| Average Case | O(n²) |
| Worst Case | O(n²) |

## Space Complexity

```text
O(1)
```

## Conclusion
After correcting the minimum index update, Selection Sort works properly and sorts the array in ascending order using constant extra space.