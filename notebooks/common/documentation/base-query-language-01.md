The **Query Language** finds all paths in a call graph that match properties described by the query applied to profiling data. It enables Hatchet’s Jupyter notebook-based interactive visualization to provide users with a simple and intuitive way to massively reduce the profiling data interactively. The **Query Language** has two dialects (Object-based Dialect and String-based Dialect), that simplify its use under diverse circumstances. 

## Category 1: Quantifier Capabilities

A valid hatchet query requires a **quantifier**. The accepted values for query node quantifiers in the Hatchet **base Query Language** are:

1. `"."`: Match a single node
2. `"*"`: Match 0 or more nodes
3. `"+"`: Match 1 or more nodes
4. `Integer`: Match an exact number of nodes


