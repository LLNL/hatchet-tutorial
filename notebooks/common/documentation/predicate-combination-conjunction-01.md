### Use intersection (AND) in query node conditions

This query type allows a user to search for nodes that meet the requirements of two or more predicates for a single quantifier. The predicates are combined using the **AND** logical operator, which means that both predicates must be satisfied by a node.

The following query matches all nodes where the `time` metric is `greater than 70000` **AND** the `name` metric `starts with MPI_`.

