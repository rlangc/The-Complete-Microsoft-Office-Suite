# Using Logical Functions: IF, AND, OR in Microsoft Excel

This guide introduces logical functions that allow your formulas to make decisions based on specific conditions.

## IF Function

Basic syntax:
```
=IF(logical_test, value_if_true, value_if_false)
```

Example:
```
=IF(A2 > 70, "Pass", "Fail")
```

## AND Function

Returns TRUE only if all conditions are true:
```
=AND(A2 > 70, B2 = "Complete")
```

Used inside IF:
```
=IF(AND(A2 > 70, B2 = "Complete"), "Pass", "Hold")
```

## OR Function

Returns TRUE if any one condition is true:
```
=OR(A2 > 70, B2 = "Complete")
```

Used inside IF:
```
=IF(OR(A2 > 70, B2 = "Complete"), "Pass", "Fail")
```

Logical functions add dynamic decision-making to your formulas, allowing you to control what values are returned based on your data.
