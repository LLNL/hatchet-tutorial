### Use Case 3: Check if numeric metric is infinity in query node predicates

Like use case 1, where certain operations on GraphFrames create nodes with NaN values, some operations can produce GraphFrame nodes with INF values. This query type covers cases where an operation on GraphFrames produce nodes with INF. 

From the graph tree and DataFrame of the dataset for this notebook, we determine that none of the nodes contain an INF. Therefore, we manually add INF to specific rows of the DataFrame below to successfully demonstrate this query type.

1. Import the Python NumPy library
2. Set the time metric of all MPI functions to INF

 
