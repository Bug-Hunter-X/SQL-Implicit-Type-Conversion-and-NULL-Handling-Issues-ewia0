# SQL Query Errors: Implicit Type Conversions and NULL Handling

This repository demonstrates common SQL errors related to implicit type conversions and the handling of NULL values.  These errors can be subtle and difficult to track down, leading to inaccurate query results or unexpected behavior.

## Implicit Type Conversion

Implicit type conversion occurs when SQL attempts to automatically convert data types during comparisons. While convenient, it can be a source of errors if the conversion fails or yields unexpected results.  The example queries highlight issues when comparing numeric columns with string literals or dates with strings of mismatched formats.

## NULL Value Handling

NULL values represent the absence of data.  Simply using `=` or other comparison operators when dealing with NULL columns will result in unexpected behavior, especially in `WHERE` clauses. The provided solution illustrates the correct use of `IS NULL`, `IS NOT NULL`, and `COALESCE` for accurate NULL handling.

## How to Run the Examples

1.  Create an SQL database.
2.  Create a table (e.g., 'employees') with the specified columns.
3.  Execute the `bug.sql` queries to observe the errors.
4.  Execute the `bugSolution.sql` queries to see the corrected versions.
