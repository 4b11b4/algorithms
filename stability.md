# Stability 
- A _sorting_ algorithm is known as "stable" iff it does not re-order objects which are equal and already adjacent.
- This is important in certain sitations, for example if we were sorting some records containing student _names_ and _GPAs_. If our records happened to be already sorted alphabetically by name and we used a _stable_ sorting algorithm to sort by GPA, then this would preserve the names in alphabetical order.
- A simpler example: 
Given an array: [2,2,1]
We would like to sort in order from lowest to highest.
If our algorithm simply swaps the first and last element, then it is not stable because the relative order of the "2s" changes.
If the algorithm put the 1 at the beginning and pushed back the 2s and thus preserving the relative order of the 2s, then the algorithm is "stable".
