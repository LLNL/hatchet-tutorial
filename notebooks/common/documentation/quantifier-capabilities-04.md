### Use Case 4: Match exact number of nodes


This query type filters a GraphFrame with the object syntax to find all query paths with an exact number of nodes, provided as an integer, that meets a query predicate.

The metric used for the query is `name` and the predicate is that the `name` metric `starts with "Calc"`. We have previously applied a query use case to match zero or more nodes that start with the name Calc. However, the user can use the following query to concisely match only those nodes that contain `exactly three nodes` that `start with name Calc`. The resulting GraphFrame should be relatively smaller, considering the original GraphFrame and the previous example.