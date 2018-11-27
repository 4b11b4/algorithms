# Floyd-Warshall Algorithm

## Warshall
f_ij(k) = R_ij(k-1) OR r_ik(k-1) AND r_kj(k-1)

## Floyd
D[i,j] <- min{ D[i,j], D[i,k], D[k,j]}

## Dijkstra
1. The most basic version of Dijkstra us distance to all notes from a single node.
Floyd's gives us an adjacency matrix from any node to any node.
Dijkstra can be modified to save the path in order to get the total distance.

2. If used linked list implementation of Dijkstra, then Floyd's actually has
better complexity (DOUBLE CHECK THIS).
