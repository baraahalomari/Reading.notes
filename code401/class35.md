# Graphs

> A graph is a non-linear data structure that can be looked at as a collection of vertices potentially connected by line segments named edges.

## Common terminology used when working with Graphs:

* Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
* Edge - An edge is a connection between two nodes.
* Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
* Degree - The degree of a vertex is the number of edges connected to that vertex.

## Directed vs Undirected

> **An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.**


```
Vertices/Nodes = {a,b,c,d,e,f}

Edges = {(a,c),(a,d),(b,c),(b,f),(c,e),(d,e),(e,f)}

```

## Directed Graphs (Digraph)

Unlike an undirected graph, a Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.

## Complete vs Connected vs Disconnected

* A connected graph is graph that has all of vertices/nodes have at least one edge.

* A disconnected graph is a graph where some vertices may not have edges.

## Acyclic vs Cyclic

* An acyclic graph is a directed graph without cycles.

* A cycle is when a node can be traversed through and potentially end up back at itself.

### Adjacency List

> An adjacency list is the most common way to represent graphs.

> An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected.

> Adjacency lists make it easy to view if one vertices connects to another.


### Weighted Graphs

A weighted graph is a graph with numbers assigned to its edges.

> When representing a weighted graph in a matrix, you set the element in the 2D array to represent the actual weight between the two paths. If there is not a connection between the two vertices, you can put a 0, although it is known for some people to put the infinity sign instead.

## Breadth First

* In a breadth first traversal, you are starting at a specific vertex/node. This node must be specified when calling the BreadthFirst() method. 
* The breadth-first traversal of a graph is like that of a tree, with the exception that graphs can have cycles. 
* Traversing a graph that has cycles will result in an infinite loop….this is bad. 
* To prevent such behavior, we need to have some way to keep track of whether a vertex has been “visited” before. Upon each visit, we’ll add the previously-unvisited vertex to a visited set, so we know not to visit it again as traversal continues.

### Algorithm :

* Enqueue the declared start node into the Queue.
* Create a loop that will run while the node still has nodes present.
* Dequeue the first node from the queue
* if the Dequeue‘d node has unvisited child nodes, add the unvisited children to visited set and insert them into the queue.

## Depth First

* In a depth first traversal, we approach it a bit different than the way we do when working with a depth first traversal of a tree. 
* Similar to how the breadth-first uses a queue, we are going to use a Stack for our depth-first traversal.

### Algorithm :

* Push the root node into the stack
* Start a while loop while the stack is not empty
* Peek at the top node in the stack
* If the top node has unvisited children, mark the top node as visited, and then Push any unvisited children back into the stack.
* If the top node does not have any unvisited children, Pop that node off the stack
repeat until the stack is empty.

## Real World Uses of Graphs

* GPS and Mapping
* Driving Directions
* Social Networks
* Airline Traffic
* Netflix uses graphs for suggestions of products

