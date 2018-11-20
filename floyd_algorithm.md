# Floyd-Warshall Algorithm

## Warshall
f_ij(k) = R_ij(k-1) OR r_ik(k-1) AND r_kj(k-1)

## Floyd
D[i,j] <- min{ D[i,j], D[i,k], D[k,j]}
