The **Query Language** finds all paths in a call graph that match properties described by the query applied to profiling data. It enables Hatchet’s Jupyter notebook-based interactive visualization to provide users with a simple and intuitive way to massively reduce the profiling data interactively. The **Query Language** has two dialects (Object-based Dialect and String-based Dialect), that simplify its use under diverse circumstances. Hatchet also supports five different categories for the **Query Language**, as shown in Fig. 1.  

|Category ID|Category Description|
|:---------:|:-------------------|
|1          |Quantifier Capabilities|
|2          |String Equivalence and Regex Matching|
|3          |String Containment (contains, starts with, ends with)|
|4          |Basic Numeric Comparison (==, >, >=, etc.)|
|5          |Comparison with Special Values (NaN, Inf, None)|

**Figure 1**: A table of the Hatchet Query Language capabilities, distinguished into categories and their corresponding cateogry ID.

Hatchet offers multiple interfaces to define queries with different trade-offs to verbosity and expressiveness. An entire catalog of queries, use cases, categories and capabilities can be found [here](https://docs.google.com/spreadsheets/d/1fKNlHmDJdDbnE4jyMcaFqdnw6ZSaexgm33rOcVAj0do/edit#gid=0).

Hatchet query language consumes a GraphFrame and a sequence of queries. Each query can comprise a **predicate** and a **quantifier**. Hatchet query language finds all **matching paths** from a provided GraphFrame. For example, in Fig.2, for the query (any with A or B), the output would comprise of 2 paths, [1, 2, 4] and [1, 3, 4].

![Graph frames and queries](../common/images/hatchet_query_graphframe.png)

**Figure 2**: A diagram to provide an overview of queries and an example of how queries filter GraphFrames.

***

## Category 2: String Equivalence and Regex Matching

Category 2 expands on query conditions by exploring string equivalence and regex matching. The Object-based Dialect of the Hatchet Query Language allows us to:

1. Check for string metric equivalence in query node predicates
2. Check for regex match on string metric in query node predicates