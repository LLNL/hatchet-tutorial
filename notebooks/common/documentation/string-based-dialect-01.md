The **String-based Dialect** is a formal language that can be used to create queries using a syntax derived from [Cypher](https://dl.acm.org/doi/10.1145/3183713.3190657). Queries generated using the **String-based Dialect** contain two main syntactic pieces: a *MATCH* statement and a *WHERE* statement. The *MATCH* statement starts with the *MATCH* keyword and defines the quantifiers and variable names used to refer to query nodes in the predicates. The *WHERE* statement starts with the *WHERE* keyword and defines one or more predicates. 

## Category 1: Quantifier Capabilities

A valid hatchet query requires a **quantifier**. The accepted values for query node quantifiers in the **String-based Dialect** are:

1. `"."`: Match a single node
2. `"*"`: Match 0 or more nodes
3. `"+"`: Match 1 or more nodes
4. `Integer`: Match an exact number of nodes 
