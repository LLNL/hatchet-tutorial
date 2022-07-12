### Use Case 5: Check if metric is None (i.e., Python keyword None) in query node predicates

Like use case 1 and 2, where certain operations on GraphFrames create nodes with NaN and INF values, respectively, some operations can produce GraphFrame nodes with None values. This query type covers cases where an operation on GraphFrames produce nodes with None. 

From the graph tree and DataFrame of the dataset for this notebook, we determine that none of the nodes contain an INF. Therefore, we manually add INF to specific rows of the DataFrame below. Before we carry on with this step, note that Python only allows object types to hold a ‘None’ value. Any other variable type automatically sets a None to NaN. To align our demonstration with this feature of Python, we apply our query only on the name metric to not interfere with any reference to the name metric carried out by the Hatcher Query Language. 

1. Create a column in the DataFrame called "name_copy" that is identical to the name column  
2. Set the name_copy metric of all MPI functions to None
 
