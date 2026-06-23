README – Kruskal's Algorithm using Disjoint Set (Union-Find)

Project Title

Implementation of Kruskal's Algorithm using Disjoint Set in Python

Description

This project implements Kruskal's Algorithm to find the Minimum Spanning Tree (MST) of a weighted, undirected graph. The algorithm uses the Disjoint Set (Union-Find) data structure to efficiently detect and avoid cycles while constructing the MST.

A Minimum Spanning Tree (MST) is a subset of the graph's edges that:

- Connects all vertices of the graph.
- Contains no cycles.
- Has the minimum possible total edge weight.

Algorithm Used

- Kruskal's Algorithm (Greedy Algorithm)
- Disjoint Set (Union-Find)

Requirements

- Python 3.x

Input Graph

edges = [
    (0, 1, 2),
    (0, 2, 3),
    (1, 2, 1),
    (1, 3, 4),
    (2, 3, 5)
]

How the Algorithm Works

1. Sort all edges in increasing order of weight.
2. Select the smallest edge.
3. Check whether adding the edge forms a cycle using Disjoint Set.
4. If no cycle is formed, add the edge to the MST.
5. Repeat until the MST contains (V - 1) edges.

MST Construction

Selected edges:

- (1, 2) → Weight = 1
- (0, 1) → Weight = 2
- (1, 3) → Weight = 4

Output

Total Cost of MST = 7

Calculation

1 + 2 + 4 = 7

Therefore,

Total Cost of MST = 7

Time Complexity

- Sorting edges: O(E log E)
- Disjoint Set operations: O(E α(V)) (almost constant time)

Overall Time Complexity:

O(E log E)

Space Complexity

O(V)

where:

- V = Number of vertices
- E = Number of edges

Applications

- Computer network design
- Road and railway network planning
- Electrical power distribution
- Telecommunication networks
- Water pipeline systems

Author

Name: Narmadha H

Department: B Tech (AI&ML)

Institution: SIMATS Enginnering