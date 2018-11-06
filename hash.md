# Hashing
## When Is It Useful
* When we are storing "Objects" rather than just "integers" or "strings"
  - For example, we have a list of keys which map to a "Student Records" obj

## Hash Function
* Should be close to constant time 
### Collissions
* Some collisions are expected. Need to deal with it.
#### Open Hashing
* Chaining
  - Implement a linked list in order to deal with collisions.
    If we have a collision at an index, we'll need to explore the linked list
    at that index until we find our element (or don't).
* Load Factor
  - If a hash function distributes keys __uniformly__, the average list of a
    linked list will be $$ a $$.
    - The ratio, $$ a = n/m $$ is called the __load factor__.
  - Ideally, $$ a $$ is kept close to 1.
    - If $$ n > m $$, open hashing still works, but is not that efficient.
#### Closed Hashing
* Keys are stored in the hash table, not in a linked list, like above.
* Does not work if $$ n > m $$.
* If lots of collisions, the array is full, thus hard to look for collisions.
  - In other words: if $$ n > m $$, it doesn't work.
##### Linear Probing
##### Double Hashing
