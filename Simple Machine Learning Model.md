
First, we  load our data using [[Pandas]]

```
import pandas as pd

data = pd.read_csv('data.csv')
```

Then we split our data into [[Features]] and [[Labels]] / Targets.

```
y = data.price

feature_cols = []

X = data[feature_cols]

```