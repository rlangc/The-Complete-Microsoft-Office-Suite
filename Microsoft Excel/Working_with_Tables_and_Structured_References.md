# Working with Tables and Structured References in Microsoft Excel

This guide explains how to convert data into Excel tables and use structured references to make formulas more readable and dynamic.

## Creating an Excel Table

1. Select your data range (including headers).
2. Press Ctrl + T or go to Insert > Table.
3. Confirm the "My table has headers" checkbox.
4. Click OK.

## Table Features

- Filterable column headers
- Automatic banded row formatting
- Auto-expansion for new data
- Total row for quick summaries

## Structured References

Excel tables use column names instead of cell references in formulas.

Example:
```
=SUM(Orders[Amount])
```

This is clearer and easier to maintain than using cell references like `=SUM(B2:B20)`.

## Naming Tables

- Click anywhere in the table.
- Go to Table Design tab > Table Name.
- Use descriptive names (e.g., SalesData, EmployeeList).

Tables improve readability, accuracy, and performance when managing datasets. Next, learn how to use logical functions like IF, AND, and OR to make decisions in your formulas.
