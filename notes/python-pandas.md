# Python: pandas Fundamentals

**Learning status:** Starter note — not assessed.

A DataFrame is a labeled two-dimensional data structure. Always inspect types and missingness before aggregating.

```python
import pandas as pd
df = pd.DataFrame({"customer": [1, 1, 2], "amount": [100, 200, 150]})
totals = df.groupby("customer", as_index=False)["amount"].sum()
print(totals)
```

## Exercise

How would you handle missing amounts without silently changing the business definition of revenue?
