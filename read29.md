# Graphs

A graph is a  non-linear data structure that consists of the following two components:

* A finite set of vertices also called as nodes.
* A finite set of ordered pair of the form (u, v) called as edge.

Some common terminology used in graphs:

1. Vertex : is a data object that can have zero or more adjacent vertices.
2. Edge : An edge is a connection between two nodes.
3. Neighbor : The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
4. Degree : The degree of a vertex is the number of edges connected to that vertex.

## Directed vs Undirected

Undirected graphs have edges that do not have a direction. The edges indicate a two-way relationship, in that each edge can be traversed in both directions. ... Directed graphs have edges with direction. The edges indicate a one-way relationship, in that each edge can only be traversed in a single direction

## Complete vs Connected vs Disconnected

The three different types are:

1. completed
2. connected
3. and disconnected.

We can say that graph is complete when all nodes are connected to all other nodes and connected when all of vertices/nodes have at least one edge. disconnected if at least two vertices of the graph are not connected by a path.

## Acyclic vs Cyclic

cyclic graph is a directed graph that contains a path from at least one node back to itself. ... An acyclic graph is a directed graph that contains absolutely no cycle; that is, no node can be traversed back to itself.

## Graph Representation

The graphs can be represented:

1. Adjacency Matrix
2. Adjacency List

## Weighted Graphs

![weighted graph](https://he-s3.s3.amazonaws.com/media/uploads/445cf8c.jpg)

It is a graph with numbers assigned to its edges and These numbers are called weights.

## Traversals

1. Breadth First
The algorithm breadth first traversal looks like:

   * Enqueue the declared start node into the Queue.
   * Create a loop that will run while the node still has nodes present.
   * Dequeue the first node from the queue
   * if the Dequeue‘d node has unvisited child nodes, add the unvisited children to visited set and insert them into the queue.

2. Depth First
The algorithm for a depth first traversal is as follows:

   * Push the root node into the stack
   * Start a while loop while the stack is not empty
   * Peek at the top node in the stack
   * If the top node has unvisited children, mark the top node as visited, and then Push any unvisited children back into the stack.
   * If the top node does not have any unvisited children, Pop that node off the stack
   * repeat until the stack is empty.

## Where to use graphs in the real life

The graphs is really important and have a lot of uses in real world:

1. GPS and Mapping
2. Driving Directions
3. Social Networks
4. Airline Traffic
5. Netflix uses graphs for suggestions of product

## Resources for this reading

1. [Graphs](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html)
