The Hatchet Query Language is a tool within Hatchet that can be used to filter, reduce, and/or prune **GraphFrame** objects for knowledge extraction. In the query language, users create expressions (called queries) that describe desired paths in a **GraphFrame**.

Every Hatchet query is made up of:
1. A Query or Query Path, which retrieves paths in a **GraphFrame** based on some specified criteria. This is essentially synonymous with the SQL term “query”. A Hatchet query is made up of a sequence of query nodes.
2. Query Nodes, which specify the criteria that must be satisfied for a part of a **GraphFrame** to match part of the query. Each query node consists of a single query node wildcard and a single query node condition.
3. Query Node Wildcards, which specify how many nodes in a **GraphFrame** should be matched to a single query node.
4. Query Node Conditions, which specify expressions that can be evaluated to boolean truth values for a given **GraphFrame** node. The truth value produced by applying a query node condition on a **GraphFrame** node is used to determine whether the **GraphFrame** node matches the corresponding query node. These are essentially synonymous with the SQL term “predicates”.

***