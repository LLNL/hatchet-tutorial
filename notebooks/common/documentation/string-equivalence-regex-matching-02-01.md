### Use Case 2: Check for regex match on string metric in query node predicates

This query type covers cases when matching a string using regex can provide an understanding of function calls with a certain string metric pattern. Object-based Dialect is used to find query nodes that match a provided regex expression. 

The notebook contains two examples for this query type. The purpose of the second example is to illustrate a relatively complex example, when compared to the first example of regex that is used to match a pattern on the `name` metric.

**Example 1:**

The following query matches all single nodes where the metric `name` matches the regex expression `MPI_.*`. The expression translates to matching nodes with the `name` metric starting with `MPI_`.
