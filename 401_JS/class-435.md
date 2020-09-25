### Graphs

> Graph: a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

***Terms:***

* **Vertex:** a data object that can have zero or more adjacent vertices

* **Edge:** a connection between two nodes

* **Neighbor:** adjacent node (i.e., connected via an edge)

* **Degree:** the number of deges connected to that vertex

---

***Types of Graphs:***

**Directed vs Undirected**

*Undirected:* a graph where each edge is undirected or bi-directional.  This type of graph does not move in any direction

*Directed (Digraph):* a graph where every edge is directed.  This type of graph has direction, as each node is directed at another node with a specific requirement of what node should be referenced next (like a linked list)

**Complete vs Connected vs Disconnected**

*Complete:* all nodes are connected to all other nodes

*Connected:*  all vertices/nodes have at least one edge
  - A *tree* is an example of a connected graph

*Disconnected:* some vertices may not have edges.  Stand alone nodes may exist

**Acyclic vs Cyclic**

* **cycles:** when a node can be traversed through and potentially end up back at itself
  - a path of positive length that starts and ends at the same vertex

*Acyclic:*  a directed graph *without* cycles
  - A *tree* is considered a DAG: directed acyclic graphy

*Cyclic:* a directed graph *with* cycles

---

**Representation**

*Adjacency Matrix:*  2-dimensional array of size nxn, where n = the number of vertices in the graph.
  - each row and column represent each vertex of the data structure
    - if an edge connects the two vertices, that space in the matrix = 1
    - if there is no connection, that space in the matrix = 0

- A graph with many connections is considered **dense**.  One with few connections is considered **sparse**

- The adjacency matrix of an undirected graph will always be symmetric

*Adjacency List:* a collection of linked lists or array that lists all other vertices that are connected.

---

**Weighted Graphs**

- A graph with numbers (weights) assigned to its edges

- In a matrix, the element in the array is set to represent the actual weight between the two paths (rather than being set automatically to 1 in the case of a connection)
  - Unconnected vertices can still be set to 0, or infinity

- In an adjacency list, both the weight and the anme of each adjacent vertex must be indicated

---

**Traversals**

*Breadth First:*
  - start at a specific vertex/node, which must be specified when calling the method
  - similar to a tree traversal *except* that cycles must be handled
    - cycles must be flagged so that we can specify whether or not they have already been traversed once - this is to prevent infinite looping within the cycle

Steps of Traversal:  
1.  Enqueue the declared start node into a Queue
1.  Create a loop that will continue while there are nodes present in the queue
1.  Dequeue the first node in the queue
1.  If the dequeued node had unvisited child nodes, mark the unvisited children as visited and then re-insert them into the queue

Pseudocode:  

```
ALGORITHM BreadthFirst(vertex)
    DECLARE nodes <-- new List()
    DECLARE breadth <-- new Queue()
    breadth.Enqueue(vertex)

    while (breadth is not empty)
        DECLARE front <-- breadth.Dequeue()
        nodes.Add(front)

        for each child in front.Children
            if(child is not visited)
                child.Visited <-- true
                breadth.Enqueue(child)   

    return nodes;
```

*Depth First:*
  - Uses a stack rather than a queue

Steps of Traversal:  
1.  Push root node into the stack
1.  Start a while loop that will continue while the stack is not empty
1.  Peek at the top node in the stack
  *  If the top node has unvisited children, mark the top node as visited and then push any unvisited children back into the stack
  * If the top node does *not* have unvisited children, Pop that node off the stack  

---

**Use Cases**

- GPS and Mapping
- Driving Directions
- Social Networks
- Airline Traffic
- Use Graphs, pattern mapping

---

[Home](https://jchinzi.github.io/reading-notes/)