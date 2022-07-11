The **Query Language** finds all paths in a call graph that match properties described by the query applied to profiling data. It enables Hatchet’s Jupyter notebook-based interactive visualization to provide users with a simple and intuitive way to massively reduce the profiling data interactively. The **Query Language** has two dialects (Object-based Dialect and String-based Dialect), that simplify its use under diverse circumstances. 

## Category 5: Special Value Identification Predicates (NaN, Inf, None)

Category 5 expands on using query node predicates to identify and filter GraphFrame nodes with special values such as NaN, Inf, or None.

The Hatchet base Query Language allows us to check if:

1. Check if numeric metric is NaN in query node predicates
2. Check if numeric metric is not NaN in query node predicates
3. Check if numeric metric is infinity in query node predicates
4. Check if numeric metric is not infinity in query node predicates
5. Check if metric is None (i.e., Python keyword None) in query node predicates
6. Check if metric is not None (i.e., Python keyword None) in query node predicates
