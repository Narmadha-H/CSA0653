README – Prim's Algorithm for Minimum Spanning Tree (MST)

Project Title

Implementation of Prim's Algorithm using Python

Description

This project implements Prim's Algorithm to find the Minimum Spanning Tree (MST) of a weighted, undirected graph represented using an adjacency matrix.

A Minimum Spanning Tree is a subset of the graph's edges that:

- Connects all vertices.
- Contains no cycles.
- Has the minimum possible total edge weight.

Algorithm Used

Prim's Algorithm (Greedy Algorithm)

Requirements

- Python 3.x

Input Graph

graph = [
    [0, 2, 3],
    [2, 0, 1],
    [3, 1, 0]
]

How the Algorithm Works

1. Start from the first vertex.
2. Select the minimum-weight edge connecting a selected vertex to an unselected vertex.
3. Add the selected edge to the MST.
4. Repeat until all vertices are included.

Output

Total Weight of MST = 3

Example

Selected edges:

- (0,1) → Weight = 2
- (1,2) → Weight = 1

Total Weight:

2 + 1 = 3

Time Complexity

O(V²)

Space Complexity

O(V)

Applications

- Network design
- Road and railway planning
- Computer networks
- Electrical circuit design
- Telecommunication systems

Author

Name: Narmadha h

Department: B Tech (AI & ML)

Institution: SIMATS Enginnering