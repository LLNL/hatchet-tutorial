**Example 2:**

In some cases, it is necessary to constrain which nodes to match. In other cases, it may be unknown which functions are called before a particular routine.

For this second example, the first quantifier (`"."`) constrains the filter to single node with the predicate that the metric `name`, `starts with lulesh`. The second quantifier (`"."`) selects all single nodes, before only `matching zero or more nodes` that satisfy the predicate that the metric `name`, `starts with Calc`.  