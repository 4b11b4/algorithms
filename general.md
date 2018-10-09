# Notes about analyzing things with "Big O" notation

- We may say that an algorithm has the complexity of "n^2" or "f(n) E O(n^2)", but this does not tell us much about "run-time" or how long the algorithm would actually take in the real world. A more experimental analysis is needed: e.g. create multiple datasets to test with, run the algorithm, plot results with different datasets, and perform some "curve-fitting".
* Distribution of a dataset matters as well! An algorithm will take differents amount of time based on how the data is distributed in a dataset (e.g. if it is sorted already).
