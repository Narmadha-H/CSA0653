

# Experiment 2: Binary Search and Logarithmic Behavior

### Aim
To implement Binary Search and experimentally verify its logarithmic behavior by counting the number of iterations for different input sizes.

### Problem Statement
Design Binary Search and count the number of iterations required to find elements in datasets of increasing size. Interpret the pattern observed and justify its efficiency compared to linear search.

### Algorithm
1. Find the middle element of the array.
2. If the key matches, return its position.
3. If the key is smaller, search the left half.
4. If the key is larger, search the right half.
5. Repeat until the element is found or the search space becomes empty.

### Time Complexity
- Best Case: O(1)
- Average Case: O(log n)
- Worst Case: O(log n)

### Space Complexity
- O(1)

### Experimental Results

| Input Size (n) | Number of Iterations |
|---------------|---------------------|
| 10 | 4 |
| 100 | 7 |
| 1000 | 10 |
| 10000 | 14 |

### Comparison with Linear Search

| Input Size | Linear Search | Binary Search |
|------------|---------------|---------------|
| 10 | 10 | 4 |
| 100 | 100 | 7 |
| 1000 | 1000 | 10 |
| 10000 | 10000 | 14 |

### Conclusion
Binary Search demonstrates logarithmic growth, O(log n). As the dataset size increases, the number of iterations increases very slowly, making it significantly more efficient than Linear Search for large datasets.

---

## Author
**Name:** Narmadha H  
**Course:** Design and Analysis of Algorithms Laboratory  
**Department:** Computer Science and Engineering