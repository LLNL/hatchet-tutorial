The **String-based Dialect** is a formal language that can be used to create queries using a syntax derived from [Cypher](https://dl.acm.org/doi/10.1145/3183713.3190657). Queries generated using the **String-based Dialect** contain two main syntactic pieces: a *MATCH* statement and a *WHERE* statement. The *MATCH* statement starts with the *MATCH* keyword and defines the quantifiers and variable names used to refer to query nodes in the predicates. The *WHERE* statement starts with the *WHERE* keyword and defines one or more predicates. Hatchet supports eight different categories for the query language, as shown in Fig. 1.  

|Category ID|Category Description|
|:---------:|:-------------------|
|1          |Quantifier Capabilities|
|2          |String Equivalence and Regex Matching Predicates|
|3          |String Containment Predicates (contains, starts with, ends with)|
|4          |Basic Numeric Comparison Predicates (==, >, >=, etc.)|
|5          |Special Value Identification Predicates (NaN, Inf, None)|
|6          |Predicate Combination through Conjunction (AND)|
|7          |Predicate Combination through Disjunction and Complement (OR, NOT)|
|8          |Predicate Combination through Other Operations (e.g., XOR)|

**Figure 1**: A table of the Hatchet Query Language capabilities, distinguished into categories and their corresponding category ID.

Hatchet offers multiple interfaces to define queries with different trade-offs to verbosity and expressiveness. An entire catalog of queries, use cases, categories and capabilities can be found [here](https://docs.google.com/spreadsheets/d/1fKNlHmDJdDbnE4jyMcaFqdnw6ZSaexgm33rOcVAj0do/edit#gid=0).

Hatchet query language consumes a GraphFrame and a sequence of queries. Each query can comprise a **predicate** and a **quantifier**. Hatchet query language finds all **matching paths** from a provided GraphFrame. For example, in Fig.2, for the query (any with A or B), the output would comprise of 2 paths, [1, 2, 4] and [1, 3, 4].

![Graph frames and queries](../common/images/hatchet_query_graphframe.png)

**Figure 2**: A diagram to provide an overview of queries and an example of how queries filter GraphFrames.

***

## Category 1: Quantifier Capabilities

A valid hatchet query requires a **quantifier**. The accepted values for query node quantifiers in the **Object-based Dialect** are:

1. `"."`: Match a single node
2. `"*"`: Match 0 or more nodes
3. `"+"`: Match 1 or more nodes
4. `Integer`: Match an exact number of nodes 
