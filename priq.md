# Priority Queues
In the real world, we don't always have some fixed data set we want to sort.
It is often the case that our data is constantly changing. We want to be able
to dynamically add to and remove from it.

A __Priority Queue__ is an abstract data type that supports sorting of real- 
time data.

For example:
- Insertion of a new elmeent
- Deletion of an element
- Initialization (organizing initial data set)

Commonly implemented as a __heap__.

## Two Types of Heaps
1. min-heap
2. max-heap

## Height of a Heap
Since a heap is a complete binary tree, it has a smallest possible height.
The height of a complete binary tree is always $$ O(log n) $$.

## Represent a Heap as a Binary Tree
* All levels must be full or __complete__, except for the last level.

## Represent Heap as an Array
A complete binary tree can be represented as an array where:
* The root is located at position $$ n $$.
  - The left child is located at: $$ 2*n $$
  - The right child is located at: $$ 2*n + 1 $$
