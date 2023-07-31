# Factors

The bug in the previous commit was due to weights not iteratively changing when new factor subsets are introduced to the algorithm. Hashmap was used to retrieve new weights with each new subset, and the global variable *g.weights* is updated for each iteration of *factors*. 