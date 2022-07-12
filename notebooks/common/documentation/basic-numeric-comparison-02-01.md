### Use Case 2: Check for numeric metric equivalence in query node predicates

This query type covers cases where the user provides a numerical value that has an equivalence relationship with a numeric metric of the nodes. Since, the query node predicates find numeric metrics that match a numerical value exactly, it is required to set this numeric metric of all the rows of the DataFrame to their floor value. This allows for a successful application of the query even when the numeric metric has a higher precision number than the numeric value provided in the query node predicate.

For the example below, we check for time metric equivalence. Hence, we:

1. Import the NumPy library for python
2. Use the NumPy library to set the time metric of all rows of the DataFrame to their floor values


