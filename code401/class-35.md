# Graphs

Reading: [Link](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html)

## Definition

A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

### Common terminology

- **Vertex** - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
- **Edge** - An edge is a connection between two nodes.
- **Neighbor** - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
- **Degree** - The degree of a vertex is the number of edges connected to that vertex.

## Graph Classification

### Directed vs Undirected

- **Undirected Graph** - a graph where each edge is bi-directional. This means that the undirected graph does not move in any direction.

- **Directed Graph** - (aka. Digraph) Each node is directed at another node with a specific requirement of what node should be referenced next.

### Complete vs Connected vs Disconnected

- **Complete** - A graph were all nodes are connected to all other nodes.
- **Connected** - A graph where all of vertices/nodes have at least one edge.
- **Disconnected** - A graph where some vertices may not have edges.

### Acyclic vs Cyclic

A cycle is when a node can be traversed through and potentially end up back at itself.

- **Acyclic** - A directed graph without cycles. So it can be traversed and will not end up back at the root node.
- **Cyclic** - A graph that has cycles. During traversal you will potentially end up back at the root node.

## Graph Representation

We can graphically represent graphs in two ways:

- **Adjacency Matrix** - Represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix. Each Row and column represents each vertex of the data structure. The elements of both the column and the row must add up to 1 if there is an edge that connects the two, or zero if there isn’t a connection.
- **Adjacency List** - The most common way to represent graphs. An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected. Adjacency lists make it easy to view if one vertices connects to another.

## Weighted Graphs

A weighted graph is a graph with numbers assigned to its edges. These numbers are called weights.

When displaying weighted graphs as adjacency lists or matrices, include the weight number along with the name of the adjacent vertex.

## Traversal

- **Breadth First** - The breadth-first traversal of a graph is like that of a tree, with the exception that graphs can have cycles. Traversing a graph that has cycles will result in an infinite loop….this is bad. To prevent such behavior, we need to have some way to keep track of whether a vertex has been “visited” before. Upon each visit, we’ll add the previously-unvisited vertex to a visited set, so we know not to visit it again as traversal continues.
  - Use a **queue** for this traversal
      1. Enqueue the declared start node into the Queue.
      1. Create a loop that will run while the node still has nodes present.
      1. Dequeue the first node from the queue
      1. if the Dequeue‘d node has unvisited child nodes, add the unvisited children to visited set and insert them into the queue.
- **Depth First** - Use a **stack** for this traversal
    1. Push the root node into the stack
    1. Start a while loop while the stack is not empty
    1. Peek at the top node in the stack
    1. If the top node has unvisited children, mark the top node as visited, and then Push any unvisited children back into the stack.
    1. If the top node does not have any unvisited children, Pop that node off the stack
    1. repeat until the stack is empty.

## Graphs IRL

- GPS and Mapping, Driving Directions, Social Networks, Airline Traffic, Netflix uses graphs for suggestions of movies.
