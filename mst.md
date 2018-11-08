# Minimum-Cost Spanning Tree (MST)

* Used when dealing with __weighted__ graphs.
* An MST is a tree that:
  - connects all vertices
  - has the smallest possible total weight of edges

## Prim's Algorithm
* Uses an adjacency matrix.
* Naive implementation. Doesn't always return the MST.
* $$ O(V*E) $$
0. Build up a tree from scratch based on input tree.
1. Add vertex 0 (root).
2. Examine all edges.
3. Add smallest edge and vertex associated with it.
4. We now have a new tree.
5. Go back to step 2. Repeat until all vertices added.

### Prim's Algorithm for Dense Graphs
* For very dense graphs (e.g. each vertex has at least V/2 neighbors), the
  complexity is $$ O(V^2) $$.
* There are some optimizations that can be done with Prim's algorithm when you
  are dealing with dense graphs.

### Prim's Algorithm for Sparse Graphs
* Using an adjacency matrix we can never do better than $$ O(V^2) $$ because
  that is the complexity for scanning all edges.
* When dealing with sparse graphs, we want to switch to a linked list
  implementation.
