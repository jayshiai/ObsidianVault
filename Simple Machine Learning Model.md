
First, we  load our data using [[Pandas]]

```
import pandas as pd

data = pd.read_csv('data.csv')
```

Then we split our data into [[Features]] and [[Labels]] / Targets.

```
y = data.price

feature_cols = ['age', 'milage']

X = data[feature_cols]

```

We'll then quickly review our data using `describe()` and `head()` method.

```
X.describe()
```

||age|milage|
|---|---|---|
|count|6557.000000|6557.000000|
|mean|3.886390|27659.219003|
|std|1.310336|15121.061173|
|min|0.183436|31.000000|
|25%|3.041752|16222.000000|
|50%|3.849418|25120.000000|
|75%|4.643395|37225.000000|
|max|10.308008|89336.000000|

