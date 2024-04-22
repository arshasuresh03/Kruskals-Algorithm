# Kruskals-Algorithm
Kruskal's algorithm: Builds a minimum spanning tree by greedily selecting edges with the smallest weight, avoiding cycles.

Kruskal's algorithm is a greedy algorithm used to find the minimum spanning tree (MST) of a connected, undirected graph. It works by sorting the edges in non-decreasing order of their weights and then adding them to the MST one by one, avoiding cycles. Kruskal's algorithm maintains a forest of trees and combines them into a single tree by selecting the smallest edge that connects two disjoint trees until all vertices are included in the MST. This algorithm is efficient for sparse graphs and has a time complexity of O(E log V), where E is the number of edges and V is the number of vertices in the graph.

Here's a step-by-step description of Kruskal's algorithm:

Initialization:
Create an empty set to store the edges of the minimum spanning tree (MST).
Initialize each vertex as a separate component (tree) in a forest.

Sort Edges:
Sort all the edges of the graph in non-decreasing order of their weights. This can be achieved using any sorting algorithm with a time complexity of O(E log E), where E is the number of edges.

Iterate Over Sorted Edges:
Iterate through the sorted list of edges.

Selecting Edges:
For each edge, check if adding it to the MST would create a cycle. This can be done by checking if the vertices of the edge belong to the same component (tree) in the forest. If adding the edge does not create a cycle, add it to the MST and merge the components (trees) containing its vertices.

Merge Components:
If the vertices of the selected edge belong to different components, merge the components by performing a union operation. This operation ensures that the vertices of the edge become part of the same component (tree) in the forest.

Repeat:
Repeat steps 4 and 5 until there are V - 1 edges in the MST, where V is the number of vertices in the graph.

Termination:
The algorithm terminates when the MST contains V - 1 edges, and all vertices are connected.

Output:
The output is the set of edges that form the minimum spanning tree (MST) of the graph.

DEMO:

![image](https://github.com/arshasuresh03/Kruskals-Algorithm/assets/160167081/a6247b97-015d-46bd-b661-0525145154ba)
