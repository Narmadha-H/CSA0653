# Warehouse Delivery Route Optimization Using Prim's Algorithm

## Project Title

Warehouse Delivery Route Optimization Using Prim's Algorithm (Greedy Strategy)

## Objective

The objective of this project is to determine the minimum-cost routes connecting multiple warehouses so that goods can be transported efficiently with the least possible transportation cost.

## Problem Statement

A logistics company operates several warehouses connected by roads. Each road has an associated transportation cost or distance. The company needs to connect all warehouses while minimizing the total delivery cost.

This problem is solved using **Prim's Algorithm**, a greedy algorithm that finds the **Minimum Spanning Tree (MST)** of a graph.

## Algorithm Used

**Prim's Algorithm (Greedy Strategy)**

Prim's algorithm starts from one warehouse and repeatedly selects the minimum-cost edge that connects a selected warehouse to an unselected warehouse until all warehouses are connected.

## Technologies Used

* Programming Language: Python 3
* Algorithm: Prim's Algorithm
* Data Structure: Adjacency Matrix

## Input Graph

```python
graph = [
    [0, 2, 4],
    [2, 0, 1],
    [4, 1, 0]
]
```

## Warehouse Representation

| Warehouse Number | Description           |
| ---------------- | --------------------- |
| 0                | Central Warehouse     |
| 1                | Distribution Center A |
| 2                | Distribution Center B |

## Expected Output

```text
Selected Routes:
Warehouse 0 --> Warehouse 1 : Distance = 2
Warehouse 1 --> Warehouse 2 : Distance = 1

Total Weight of MST = 3
```

## Working Procedure

1. Start from Warehouse 0.
2. Select the minimum-cost edge connecting a selected warehouse to an unselected warehouse.
3. Add the selected edge to the Minimum Spanning Tree.
4. Repeat the process until all warehouses are connected.
5. Calculate the total transportation cost.

## Advantages

* Minimizes transportation cost.
* Reduces delivery time.
* Avoids unnecessary routes.
* Efficient for logistics and distribution networks.

## Applications

* Warehouse distribution systems
* Delivery route planning
* Transportation networks
* Communication networks
* Power distribution systems

## Time Complexity

O(V²)

Where V is the number of warehouses.

## Space Complexity

O(V)

## Conclusion

The Warehouse Delivery Route Optimization System successfully uses Prim's Algorithm to determine the minimum-cost network connecting all warehouses. The algorithm ensures efficient resource utilization and minimizes the total transportation cost, making it highly suitable for logistics and supply chain management applications.
