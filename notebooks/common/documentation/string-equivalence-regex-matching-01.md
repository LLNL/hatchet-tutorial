### Use Case 1: Check for string metric equivalence in query node conditions


This query type covers cases when comparing string equivalence to filter a graph tree is helpful. Object-based Dialect is used to find query nodes that are equivalent to a provided string metric. The following query matches all single nodes where the metric used for the query predicate is `name` and the equivalent string to find is `MPI_Finalize`. 

Note: The query condition to find string metric equivalence can be written as `{"metric_name": "string_to_check"}`.
