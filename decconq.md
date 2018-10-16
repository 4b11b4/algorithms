# Decrease & Conquer 
* Known as the "__inductive__" approach because:
 - The idea is to __recursively__ attack the problem by breaking it into smaller pieces.
<br>
* A basic real world example: exponentiation
 - go back through slides an add figures 4.1, 4.2
  - Figure 4.1
    - $$ a^n = a^n-1 * n $$ for all integers $$ n > 0 $$
    - This isn't any better than brute force. It has the same structure as a __for loop__.
  - Figure 4.2
    - Here you get a logn complexity. It should be obvious from the pattern of $$ (n/2)^2 $$ that we will get $$ logn $$.
