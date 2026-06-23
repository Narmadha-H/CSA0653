## Experiment 1: Merge Sort and Memory Usage Analysis

### Aim
To implement the Merge Sort algorithm and analyze its memory usage during execution.

### Problem Statement
Implement Merge Sort and record the auxiliary space required for different input sizes. Interpret how additional memory impacts performance and justify the trade-off between time and space complexity.

### Algorithm
1. Divide the array into two equal halves.
2. Recursively sort the left and right halves.
3. Merge the sorted halves into a single sorted array.
4. Repeat until the entire array is sorted.

### Time Complexity
- Best Case: O(n log n)
- Average Case: O(n log n)
- Worst Case: O(n log n)

### Space Complexity
- Auxiliary Space: O(n)

### Observation Table

| Input Size (n) | Auxiliary Space |
|---------------|----------------|
| 10 | 10 elements |
| 100 | 100 elements |
| 1000 | 1000 elements |
| 10000 | 10000 elements |

### Conclusion
Merge Sort requires additional memory proportional to the input size (O(n)). Although it uses extra space, it provides efficient and predictable performance with a time complexity of O(n log n), making it suitable for large datasets.

---
