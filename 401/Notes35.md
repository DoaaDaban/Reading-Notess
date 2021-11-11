# Graphs

A graph is a non-linear data structure that can be looked at as a collection of `nods` that call `vertices` potentially connected by line segments named `edges`.

## Common terminology used when working with Graphs:

1. `Vertex`: A vertex, also called a **nod**, is a data object that can have zero or more adjacent vertices.

2. `Edge`: An edge is a connection between two nodes.

3. `Neighbor`: The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.

4. `Degree`: The degree of a vertex is the number of edges connected to that vertex.

![graph](https://adrianmejia.com/images/graph-parts.jpg)

### Types of graphs:

1. Undirected Graphs

It is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.

![Undirected Graphs](https://cdncontribute.geeksforgeeks.org/wp-content/uploads/undirectedgraph.png)

2. Directed Graphs (Digraph)

It Has a direction so eache vertex is directed at another vertex with a specific requirement of what vertex should be referenced next.

![Directed Graphs](https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/Directed_graph.svg/1280px-Directed_graph.svg.png)

## Complete vs Connected vs Disconnected

The type of graph depends on how connected the graphs are to other vertices.

1. Complete Graphs

A complete graph is when all nodes are connected to all other nodes.

![Complete Graphs](https://www.researchgate.net/publication/318598613/figure/fig1/AS:660446189219841@1534474050479/The-complete-graph-K-6.png)

2. Connected

A connected graph is graph that has all of vertices have at least one edge.

![Connected](https://www.tutorialspoint.com/discrete_mathematics/images/connected_graph.jpg)

3. Disconnected

 A disconnected graph is a graph where some vertices may not have edges.

![Disconnected](https://i.stack.imgur.com/xCOe9.png)