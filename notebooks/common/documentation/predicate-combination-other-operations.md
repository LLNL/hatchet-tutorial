### Use more complex logic than AND, OR, and NOT in query node predicates 

This query type allows a user to search for nodes that meet the requirements of a complex logical operator, specifically `XOR` for this example. The predicates are combined using the XOR logical operator, which means that `only one` of the two predicates must be satisfied by a node. One can apply an XOR logic to predicates by using the following combination of AND, OR, and NOT logical operators:

(predicate 1 **AND** **NOT** predicate 2) **OR** (**NOT** predicate 1 **AND** predicate 2)

The following query matches all nodes where either the `name` metric `starts with MPI_` **AND** the `time` metric `is NOT less than 10000` **OR** the `name` metric does `NOT start with MPI_` **AND** the `time` metric `is less than 10000`. In this way, we accomplish the application of an `XOR` logical operation on the query node predicates such that:

* the `name` metric `starts with MPI_` **XOR** the `time` metric `is less than 10000`