# E-Commerce Product Sorting System using Merge Sort

## Problem Statement
An e-commerce platform must sort millions of products based on price and ratings to ensure fast user access. The system should efficiently handle large datasets while maintaining stability and scalability.

## Objective
To implement Merge Sort for sorting products and analyze its performance, memory usage, and suitability for large-scale applications.

## Why Merge Sort?
- Stable sorting algorithm.
- Guarantees O(n log n) time complexity.
- Suitable for large datasets and external sorting.
- Maintains the order of products having the same price or rating.

## Divide and Conquer Approach
1. Divide the product list into two halves.
2. Recursively sort both halves.
3. Merge the sorted halves into one sorted list.

## Algorithm
1. If the array contains one element, return it.
2. Divide the array into two equal parts.
3. Recursively sort the left and right halves.
4. Merge the sorted halves.

## Time Complexity

| Case | Complexity |
|------|------------|
| Best Case | O(n log n) |
| Average Case | O(n log n) |
| Worst Case | O(n log n) |

## Space Complexity
- Auxiliary Space: O(n)

## Challenges
- Additional memory requirement.
- Large datasets require efficient memory management.
- Merging process needs temporary arrays.

## Advantages
- Stable sorting.
- Predictable performance.
- Efficient for large-scale e-commerce systems.

## Conclusion
Merge Sort is an ideal choice for an e-commerce product sorting system because it provides consistent performance and preserves the order of equal elements, making product searching and filtering faster and more reliable.

## Author
Name: Narmadha H
Course: Design and Analysis of Algorithms Laboratory