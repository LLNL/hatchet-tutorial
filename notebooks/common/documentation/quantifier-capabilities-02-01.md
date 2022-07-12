### Use Case 2: Match zero or more nodes

In many cases, a user may not know how many nodes to match. For this reason, hatchet provides the `"*"` and `"+"` literals as a quantifier `match zero or more nodes` and `match one or more nodes`, respectively.

This query type filters a GraphFrame with the object syntax to find all query paths with zero or more nodes that meet a query predicate. This notebook contains two examples for this query use case. The purpose of the second example is to illustrate the difference between the query use cases that `match zero or more nodes` and `match one or more nodes`.

**Example 1:**

For the first example, the following query matches all zero or more nodes where the predicate that the `name` metric `starts with "Calc"` is satisfied.
