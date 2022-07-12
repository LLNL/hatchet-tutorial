### Use Case 1: Evaluate numeric metric comparison (e.g., greater than) in query node predicates


In the simplest case, a user can apply this query type to find GraphFrame nodes where the time spent on the nodes is comparable to a numerical value using inequalities (<, >, <=, >=). A practical use case of such type of query is to constrain which nodes to match before conducting a numeric metric comparison. Below, we look at an example with a similar use case.

The following query first filters all single nodes with the name metric `lulesh.cycle`. Then, the second query node includes all nodes below the lulesh.cycle node in the GraphFrame. The final query node matches single nodes in the GraphFrame where the numeric comparison is satisfied when the `time` metric `is greater than 100000`:
