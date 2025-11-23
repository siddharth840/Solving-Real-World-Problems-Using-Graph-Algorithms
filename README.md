Overview

This project focuses on the implementation of four major graph algorithms and their applications in real-world scenarios. The objective is to understand how graph concepts are used in social networking, navigation, emergency response, and infrastructure network planning.

The following four problems were solved using suitable algorithms:

Social Network Friend Suggestion – BFS / DFS

Route Planning for Google Maps – Bellman-Ford

Emergency Response Path Identification – Dijkstra

Network Cable Installation – Minimum Spanning Tree (Prim’s Algorithm)

Along with the implementation, performance profiling for execution time and memory usage was done. Visual interpretation of execution time versus graph size is also included.

Implemented Features

• BFS-based mutual friend suggestion
• Bellman-Ford shortest path with negative-weight handling and cycle detection
• Dijkstra’s algorithm using min-heap for fast emergency routing
• Minimum Spanning Tree construction using Prim’s algorithm
• Time and memory profiling for every algorithm
• Execution-time graphs generated using Matplotlib

Project Files

graph_realworld.ipynb — Jupyter Notebook containing full source code, outputs and graphs

README.md — Documentation of the assignment

requirements.txt — List of Python libraries required to run the notebook

Dataset Description

A medium-sized realistic dataset with around 20 nodes was used. Separate graph structures were created for each problem:

• Social network (undirected) for BFS
• Road network (directed, some negative weights) for Bellman-Ford
• Emergency travel map (undirected weighted) for Dijkstra
• Office cable network (sparse undirected weighted) for MST

The graphs were generated programmatically to imitate realistic connectivity levels.

How to Run the Notebook

Step 1: Install required libraries
pip install -r requirements.txt

Step 2: Open and run the notebook
jupyter notebook graph_realworld.ipynb

All cells can be executed sequentially without modification.

Results Summary
Algorithm	Time Complexity	Remarks
BFS / DFS	O(V + E)	Suitable for friend suggestion or similar contact-based recommendations
Bellman-Ford	O(V × E)	Works on graphs with negative weights and can detect negative cycles
Dijkstra	O(E log V)	Efficient for route planning with only positive weights
Prim (MST)	O(E log V)	Ideal for minimizing total infrastructure or cable installation cost

The profiling results verify that algorithms optimized with priority queues perform significantly better on larger graphs.

Conclusion

This assignment demonstrates that selecting the correct graph algorithm depends strongly on the real-world problem:

• Social media platforms rely on BFS/DFS for recommending new connections
• Navigation systems like Google Maps must handle negative penalties; hence Bellman-Ford is suitable
• Emergency services require fast path computation, making Dijkstra the best choice
• Telecom companies and network planners minimize total installation cost using MST

The project successfully bridges theoretical graph algorithms with real-world scenarios.

References

• CLRS – Introduction to Algorithms
• GeeksforGeeks – Graph Algorithms Documentation
• Python Official Documentation – collections, heapq, matplotlib
