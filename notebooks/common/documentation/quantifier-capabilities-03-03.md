Execution of the second examples for use case 2 (match zero or more nodes) and use case 3 (match one or more nodes) demonstrate the difference between the two query types when used in combination with other quantifiers and predicates. 

The predicate that the metric `name`, `starts with Calc` for this dataset demonstrates that when we `match one or more nodes`, the filter omits the node with the `name "TimeIncrement"`, as it does not satisfy the third quantifier and predicate in this example. 

This specific node is included when the third quantifier in this example is changed to match zero or more nodes instead. The query match is also reflected in the DataFrame: 
