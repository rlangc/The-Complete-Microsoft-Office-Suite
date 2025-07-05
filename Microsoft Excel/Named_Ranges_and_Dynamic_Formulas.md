# Using Named Ranges and Dynamic Formulas in Microsoft Excel

This guide shows how to create named ranges and apply dynamic formulas for clearer, more flexible spreadsheet design.

---

## What Is a Named Range?

A named range assigns a readable label to a cell or range of cells.

Creating one:
1. Select a range.
2. Go to Formulas > Define Name.
3. Enter a name (e.g., TaxRate).
4. Use the name in formulas:
```
=Subtotal * TaxRate
```

---

## Benefits

- Easier to read formulas.
- Reduces errors and improves documentation.
- Simplifies cross-sheet references.

---

## Dynamic Named Ranges

Use functions like OFFSET or INDEX with COUNTA to define ranges that grow as data is added.

Example:
```
=OFFSET(Sheet1!$A$1, 0, 0, COUNTA(Sheet1!$A:$A), 1)
```

This adjusts the range automatically as new data is entered.

---

Using named ranges helps create self-documenting, adaptable spreadsheets especially useful in large or shared workbooks.
