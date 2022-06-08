### Dropping index levels

As a precursor to defining queries, we drop the index level of the GraphFrame using the `drop_index_levels()` Hatchet function. Hatchet hierarchical indexing can be of two types, depending on whether there is a single metric per node or multiple set of metrics per node.  

If a node contains a single metric, the DataFrame will use an `Index` object containing the node column. If a node has an additional level of information, Hatchet creates a `MultiIndex` to store the information pertaining to multiple sets of metrics per node. `MultiIndex` stores the node column as the "top" level of the index, followed by additional information on the levels below. 

Based on the types of indexing (`Index or MultiIndex`), retrieving data from a DataFrame corresponding to a particular node either retrieves a single or multiple rows. This difference can cause issues when applying query node predicates.
Therefore, it is necessary to get rid of all index levels besides the node column through an aggregation operation on the GraphFrame. Then, a query node predicate can be applied to the GraphFrame. 