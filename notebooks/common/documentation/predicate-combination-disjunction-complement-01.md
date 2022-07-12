### Use Case 1: Use union (OR) in query node predicates

This query type allows a user to search for nodes that meet the requirements of two or more predicates for a single quantifier. The predicates are combined using the OR logical operator, which means that at least one of the predicates must be satisfied by a node.

The following query matches all nodes where the `name` metric `starts with MPI_` **OR** the `name` metric `starts with Lagrange`.
