The **String-based Dialect** is a formal language that can be used to create queries using a syntax derived from [Cypher](https://dl.acm.org/doi/10.1145/3183713.3190657). Queries generated using the **String-based Dialect** contain two main syntactic pieces: a *MATCH* statement and a *WHERE* statement. The *MATCH* statement starts with the *MATCH* keyword and defines the quantifiers and variable names used to refer to query nodes in the predicates. The *WHERE* statement starts with the *WHERE* keyword and defines one or more predicates. 

## Category 3: String Containment Predicates (contains, starts with, ends with)

Category 3 expands on a user-friendly alternative to using regex in query node predicates to check for string metrics that match a certain substring. This alternative method is exclusive to Hatchet's base Query Language and it's String-based dialect, providing a simpler approach to defining query node predicates and removing dependency on regex knowledge.

The String-based Dialect of the Hatchet Query Language allows us to `check if string metric`:

1. Starts with substring in query node predicates
2. Ends with substring in query node predicates
3. Contains substring in query node predicates 
