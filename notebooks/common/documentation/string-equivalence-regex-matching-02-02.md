**Example 2:**

In some cases, one is aware that the functions to search for `starts with` and `ends with` a certain string value. This example provides a scenario where the user knows to search functions that `end with Elems`, then further restrict the query to only include functions that `start with Apply or Calc`.

The following query matches all single nodes where the metric `name` matches the regex expression `(Apply|Calc).*Elems$`. The expression translates to matching nodes with the `name` that starts with either `Apply or Calc` and ends with `Elems`.