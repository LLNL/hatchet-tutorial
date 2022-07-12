The **Query Language** finds all paths in a call graph that match properties described by the query applied to profiling data. It enables Hatchet’s Jupyter notebook-based interactive visualization to provide users with a simple and intuitive way to massively reduce the profiling data interactively. The **Query Language** has two dialects (Object-based Dialect and String-based Dialect), that simplify its use under diverse circumstances. 

## Category 3: String Containment Predicates (contains, starts with, ends with)

Category 3 expands on a user-friendly alternative to using regex in query node predicates to check for string metrics that match a certain substring. This alternative method is exclusive to Hatchet's base Query Language and it's String-based dialect, providing a simpler approach to defining query node predicates and removing dependency on regex knowledge.

The Hatchet base Query Language allows us to `check if string metric`:

1. Starts with substring in query node predicates
2. Ends with substring in query node predicates
3. Contains substring in query node predicates

