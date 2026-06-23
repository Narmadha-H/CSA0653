# Real-Time Ranking System using Quick Sort

## Problem Statement
A real-time ranking system continuously updates user scores and requires fast sorting for leaderboard display.

## Objective
To implement Quick Sort and analyze its performance under different input conditions.

## Why Quick Sort?
- Very fast in practice.
- In-place sorting algorithm.
- Requires less memory.
- Suitable for frequently changing datasets.

## Divide and Conquer Approach
1. Select a pivot element.
2. Partition the array into smaller and larger elements.
3. Recursively sort both partitions.
4. Combine the results.

## Algorithm
1. Choose a pivot.
2. Partition the array around the pivot.
3. Apply Quick Sort to the left partition.
4. Apply Quick Sort to the right partition.

## Time Complexity

| Case | Complexity |
|------|------------|
| Best Case | O(n log n) |
| Average Case | O(n log n) |
| Worst Case | O(n²) |

## Space Complexity
- O(log n)

## Challenges
- Choosing an efficient pivot.
- Dynamic score updates.
- Worst-case performance on sorted data.

## Optimized Approach
Use **Randomized Pivot Selection**:
- Select the pivot randomly.
- Reduces the chance of worst-case partitions.
- Improves average performance.

## Performance Evaluation

| Input Type | Performance |
|------------|-------------|
| Random Data | O(n log n) |
| Sorted Data | O(n²) |
| Randomized Pivot | Near O(n log n) |

## Advantages
- Fast execution.
- Low memory usage.
- Suitable for real-time applications.

## Conclusion
Quick Sort with randomized pivot selection is highly effective for real-time ranking systems because it provides fast average performance and efficiently handles frequent updates in leaderboards.

## Author
Name: Narmadha H
Course: Design and Analysis of Algorithms Laboratory