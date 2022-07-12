The **String-based Dialect** is a formal language that can be used to create queries using a syntax derived from [Cypher](https://dl.acm.org/doi/10.1145/3183713.3190657). Queries generated using the **String-based Dialect** contain two main syntactic pieces: a *MATCH* statement and a *WHERE* statement. The *MATCH* statement starts with the *MATCH* keyword and defines the quantifiers and variable names used to refer to query nodes in the predicates. The *WHERE* statement starts with the *WHERE* keyword and defines one or more predicates. 

## Category 5: Special Value Identification Predicates (NaN, Inf, None)

Category 5 expands on using query node predicates to identify and filter GraphFrame nodes with special values such as NaN, Inf, or None.

The String-based Dialect of the Hatchet Query Language allows us to check if:

1. Check if numeric metric is NaN in query node predicates
2. Check if numeric metric is not NaN in query node predicates
3. Check if numeric metric is infinity in query node predicates
4. Check if numeric metric is not infinity in query node predicates
5. Check if metric is None (i.e., Python keyword None) in query node predicates
6. Check if metric is not None (i.e., Python keyword None) in query node predicates 
