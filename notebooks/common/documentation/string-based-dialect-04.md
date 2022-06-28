The **String-based Dialect** is a formal language that can be used to create queries using a syntax derived from [Cypher](https://dl.acm.org/doi/10.1145/3183713.3190657). Queries generated using the **String-based Dialect** contain two main syntactic pieces: a *MATCH* statement and a *WHERE* statement. The *MATCH* statement starts with the *MATCH* keyword and defines the quantifiers and variable names used to refer to query nodes in the predicates. The *WHERE* statement starts with the *WHERE* keyword and defines one or more predicates. 

## Category 4: Basic Numeric Comparison Predicates (==, >, >=, <, <=)

Category 4 expands on query conditions by exploring predicates that compare numerical metrics of performance data. An example of a numerical metric is "time". The Object-based Dialect of the Hatchet Query Language allows us to:

1. Evaluate numeric metric comparison (e.g., greater than) in query node predicates
2. Check for numeric metric equivalence in query node predicates
