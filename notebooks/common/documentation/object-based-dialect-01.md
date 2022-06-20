The **Object-based Dialect** is a formal language that is built around Python’s built-in objects. Queries are composed using Python’s list, tuple, and dict built-in data structures within **Object-based Dialect** of Hatchet query language.

## Category 1: Quantifier Capabilities

A valid hatchet query requires a **quantifier**. The accepted values for query node quantifiers in the **Object-based Dialect** are:

1. `"."`: Match a single node
2. `"*"`: Match 0 or more nodes
3. `"+"`: Match 1 or more nodes
4. `Integer`: Match an exact number of nodes
