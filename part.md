# Partitioning

* 3 Inputs:
1. array, a
2. left index, L
3. right index, R

* 1 Output:
1. an index, I

* The basic idea:
- Split a list in half (but don't sort all the way).
 - But __at least know__ that...
  - Elements $$ a[L]..a[I] < a[I] $$
    and
  - Elements $$ a[I]..a[R] > a[I] $$

# Complexity
- Hoare Partition (Turing Award)
 - This is quicksort.
- Lomuto Partition
  ![lomuto](lomuto.gif)
  Lomuto's algorithm is "simpler, but less efficient". (UNVERIFIED)

# Applications
1. Selection Problem
 * utilizes partitioning to make finding the median value $$ \in O(n) $$
 * worst case
   When the array is already sorted?
 * best case:
   The best case occurs when the array is "perfectly balanced" or, in other words, when we recurse we always split the array in half.

# QuickSort vs QuickSelect Complexity
Best Case:
 - QuickSort:
   $$ T(n) = n + 2*T(n/2) $$
 - QuickSelect:
   $$ T(n) = n + T(n/2) $$
Worst Case:
 - When the array is already sorted...
   but instead of picking our pivot as the first or last value, we can pick the median of three values and then we do not run into the worst case. Picking a random number is the best idea.
