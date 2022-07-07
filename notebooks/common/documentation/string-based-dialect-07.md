The **String-based Dialect** is a formal language that can be used to create queries using a syntax derived from [Cypher](https://dl.acm.org/doi/10.1145/3183713.3190657). Queries generated using the **String-based Dialect** contain two main syntactic pieces: a *MATCH* statement and a *WHERE* statement. The *MATCH* statement starts with the *MATCH* keyword and defines the quantifiers and variable names used to refer to query nodes in the predicates. The *WHERE* statement starts with the *WHERE* keyword and defines one or more predicates. 

## Category 7: Predicate Combination through Disjunction and Complement (OR, NOT)

Category 7 expands on combining query predicates through disjunction with the `OR` logical operator and taking the complement of query predicates using the `NOT` logical operator.

The String-based Dialect of the Hatchet Query Language allows us to use:

1. Union (OR) in query node predicates
2. Negation (NOT) in query node predicates
