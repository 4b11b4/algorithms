# Partitioning

* 3 Inputs:
1. array, a
2. left index, L
3. right index, R

* 1 Output:
1. an index, I

* The basic idea:
- Split a list in half (but don't sort).
 - But __at least know__ that...
  - Elements below a[I] < a[I]
    and
  - Elements above a[I] > a[i]

## Example:
1. The function returns the index of the __median__ element after searching the entire array.
2. You could then use this return value 

# Complexity
* $$ O(n) $$... powerful
- Hoare Partition (Turing Award)
 - This is quicksort.
- Lomuto Partition
  ![lomuto](lomuto.gif)
  Lomuto's algorithm is "simpler, but less efficient". (UNVERIFIED)

# Applications
1. Selection Problem
 * utilizes partitioning to make finding the median value $$ in O(n) $$
