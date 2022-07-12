### Use Case 2: Check if string metric ends with substring in query node predicates


This type of query provides an understanding of function calls that `end with` a certain substring provided by the user. The String-based Dialect and the base Query Language facilitate this query type with a `'ENDS WITH'` keyword and `endswith` function, respectively. This notebook contains two examples for this query use case. The purpose of the second example is to illustrate a relatively complex example of a query that is comparable to the notebook example on string regex matching.

**Example 1:**

For the first example, the following query checks for all single nodes with the name metric that `ends with Elems`: