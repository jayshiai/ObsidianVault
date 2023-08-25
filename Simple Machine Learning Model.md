
First, we  load our data using [[Pandas]]
(Here we are using cars data I scrapped)

```
import pandas as pd

data = pd.read_csv('data.csv')

data
#Use of print(data) is also valid
```

| |make|model|price|age|milage|colour|fuel|transmission|body|location|
|---|---|---|---|---|---|---|---|---|---|
|0|PEUGEOT|108 HATCHBACK 1.2 VTi Allure 5dr|6250|8.071184|65454|Mauve|Petrol|Manual|Hatchback|Norwich|
|1|SKODA|CITIGO HATCHBACK 1.0 MPI SE 3dr|6300|7.255305|51817|White|Petrol|Manual|Hatchback|Sheffield|
|2|FIAT|500 HATCHBACK 1.2 Pop Star 3dr|6500|7.170431|58879|Grey|Petrol|Manual|Hatchback|Manchester|
|3|CITROEN|C1 HATCHBACK 1.0 VTi Flair 3dr|7000|8.876112|23262|Orange|Petrol|Manual|Hatchback|Doncaster|
|4|VAUXHALL|VIVA HATCHBACK 1.0 SE 5dr [A/C]|7000|6.004107|46730|White|Petrol|Manual|Hatchback|Swindon|
|...|...|...|...|...|...|...|...|...|...|...|
|6552|MERCEDES-BENZ|GLC COUPE GLC 300 4Matic AMG Line 5dr 9G-Tronic|39750|2.376454|26367|Silver|Petrol|Automatic|FourByFour|Nottingham|
|6553|MERCEDES-BENZ|GLC DIESEL COUPE GLC 300de 4Matic AMG Line 5dr...|40000|2.198494|30526|Grey|Hybrid|Automatic|FourByFour|Cardiff|
|6554|VOLKSWAGEN|TOUAREG DIESEL ESTATE 3.0 V6 TDI 4Motion R-Lin...|40000|3.696099|21874|Black|Diesel|Automatic|FourByFour|Bristol|
|6555|AUDI|Q8 DIESEL ESTATE 50 TDI Quattro S Line 5dr Tip...|42000|2.973306|60639|Silver|Diesel|Automatic|FourByFour|Nottingham|
|6556|AUDI|RS 5 COUPE SPECIAL EDITION RS 5 TFSI Quattro A...|43000|3.926078|47000|White|Petrol|Automatic|Coupe|Wakefield|

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

|age|milage|
|---|---|---|
|count|6557.000000|6557.000000|
|mean|3.886390|27659.219003|
|std|1.310336|15121.061173|
|min|0.183436|31.000000|
|25%|3.041752|16222.000000|
|50%|3.849418|25120.000000|
|75%|4.643395|37225.000000|
|max|10.308008|89336.000000|


```
X.head()
```

| |age|milage|
|---|---|---|
|0|8.071184|65454|
|1|7.255305|51817|
|2|7.170431|58879|
|3|8.876112|23262|
|4|6.004107|46730|


Now that we have loaded, split and analyzed our data , we can start building our model.


# Building our model

To build our model, we'll be using [[scikit-learn]] library. It is the most popular library for modeling data stored in DataFrames.