# Priority Queues
In the real world, we don't always have some fixed data set we want to sort.
It is often the case that our data is constantly changing. We want to be able
to dynamically add to and remove from it.

A __Priority Queue__ is an abstract data type that supports sorting of real 
time data.

For example:
- Insertion of a new elmeent
- Deletion of an element
- Initialization (organizing initial data set)

A __Priority Queue__ is commonly implemented as a __heap__.

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

## Operations on a Heap
### Heap Properties
* To understand why these are the operations for a "heap", we first should
  define 3 properties of "heaps" or "priority queues":
### Operations
* fixUp()
  - worst case: $$ O(logn) $$ because max height of bin tree = $$ logn $$
* fixDown()
* insert()
  - put at end of array (a heap fills from left to right)
  - makes a call to fixUp() -- if necessary
* delete()
  - we only ever delete the max element (the root)
  - calls fixDown()
* initialization()
  - two methods:
    1. top-down
      - $ O(nlogn) $$ time
      - $ O(n) $$ extra space
    2. bottom-up
      - $$ O(n) $$ time
      - $$ O(1) $$ extra space
      - start at index N/2 in the array, because we don't need to fixDown()
        the leaves

## HeapSort
* add a visualization here
