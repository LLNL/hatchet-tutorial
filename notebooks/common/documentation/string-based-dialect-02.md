The **String-based Dialect** is a formal language that can be used to create queries using a syntax derived from [Cypher](https://dl.acm.org/doi/10.1145/3183713.3190657). Queries generated using the **String-based Dialect** contain two main syntactic pieces: a *MATCH* statement and a *WHERE* statement. The *MATCH* statement starts with the *MATCH* keyword and defines the quantifiers and variable names used to refer to query nodes in the predicates. The *WHERE* statement starts with the *WHERE* keyword and defines one or more predicates. 

## Category 2: String Equivalence and Regex Matching

Category 2 expands on query conditions by exploring string equivalence and regex matching. The String-based Dialect of the Hatchet Query Language allows us to:

1. Check for string metric equivalence in query node predicates
2. Check for regex match on string metric in query node predicates
