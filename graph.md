# Graph Theory
## Introduction to Graphs
 What is a __graph__? A way to represent something.
* A graph is made up of:
 - __vertices:__ "nodes" or "circles", and...
 - __edges:__ the lines

* Each vertex has a __degree__ or "number of connections": the number of edges that connect to it.
 - The sum of degrees (the sum of connections) is (insert sum here) $$ = 2E $$

* A graph can be represented mathematically by $$ G=(V,E) $$  where V and E are a list of vertices and edges.

* A __path__ is a list of vertices.
 - A __path__ can be written mathematically as:
   $$ \{v0, v1, v2, etc\} \in E $$
   The $$ \in E $$ part says that it is mathematically possible to get from point $$ v_0 $$ to $$ v_n $$.


* When talking about graph theory, the word __cycle__ is used.
 - In an __undirected__ graph, the length of a __cycle__ must be at least 3. (you have to move three times to get back to where you started)
 - It is possible that a graph is __acyclic__ or does not have any possible cycles.
 - In a __directed__ graph, the length of a cycle could just be 1.

* A __graph__ may be __directed__ or __undirected__.
 - In __directed graphs__, all arrows point forward.

* The words, "__strongly connected__", mean that in directed graphs, it is possible to travel from one node to another.
 - In directed graphs, it may be useful to break up the graph into a list of "__strongly connected__" graphs.

* Trees
- A tree is a connected, acyclic graph.
- *Fun* fact: if you add one edge to a tree, it is possible to have a cycle.
- When we say that it is "connected", it means there is a possible to path to any node. There does not exist any nodes which are isolated.

* Forest
- Any graph can be broken down into it's connected components.

* DAG 
- Similar to a tree, but different?

* Representing a graph inside of a computer:
 - adjacency matrix g[i][j]: an entry of 1 means there is a connection between vertices i and j
  - uses space $$ =V^2 $$
  - if our matrix does not have many connections, or edges, then we will be wasting a lot of space
  - to determine if something is connected, this can be examined in constant time
 - adjacency list: use a linked list
  - uses space $$ =V*E $$
  - to determine if something is connected... well then we have to "traverse" the until we get there...

## Graph Traversal Algorithms
* Depth First Search (DFS)
 - Traverses down a stack and explores all possible connections.
 - Uses a stack.
 - Visual Learners: YouTube Link
 - Can be used to check for __connectivity__ and __acyclicy__
 - matrix: O(V^2)
 - list: O(V+E)
* Breadth First Search (BFS)
 - Searches all nodes at each connection distance.
 - Uses a queue.
 - Visual Learners: YouTube Link
 - matrix: O(V^2)
 - list: O(V+E)
 - Same complexity as DFS for data types.
* Topological Sorting
 - For a directed graph, there cannot be a cycle.
 - Just take the stack in reverse? After using DFS?
 - Visual Learners: YouTube Link
