#documentation #sklearn #Machine_Learning 

# Ordinal Encoding
Categorical values with defined hierarchy. Called __ordinal variables__ 
![[Pasted image 20230909154205.png]]

# One-Hot Encoding
No defined hierarchy. Called __nominal variables__
![[Pasted image 20230909154218.png]]

# Training the model
We use the [`OneHotEncoder`](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.OneHotEncoder.html) class from scikit-learn to get one-hot encodings. There are a number of parameters that can be used to customize its behavior.

- We set `handle_unknown='ignore'` to avoid errors when the validation data contains classes that aren't represented in the training data, and
- setting `sparse=False` ensures that the encoded columns are returned as a numpy array (instead of a sparse matrix).

```python
from sklearn.preprocessing import OneHotEncoder

  

OH_encoder = OneHotEncoder(handle_unknown='ignore', sparse=False)

  

# Apply one-hot encoder to each column with categorical data

object_cols = ["make","fuel","transmission","body"]

OH_cols_train = pd.DataFrame(OH_encoder.fit_transform(train_X[object_cols]))

OH_cols_valid = pd.DataFrame(OH_encoder.transform(val_X[object_cols]))

  

# One-hot encoding removed index; put it back

OH_cols_train.index = train_X.index

OH_cols_valid.index = val_X.index

  

# Remove categorical columns (will replace with one-hot encoding)

num_X_train = train_X.drop(object_cols, axis=1)

num_X_valid = val_X.drop(object_cols, axis=1)

  

# Add one-hot encoded columns to numerical features

OH_X_train = pd.concat([num_X_train, OH_cols_train], axis=1)

OH_X_valid = pd.concat([num_X_valid, OH_cols_valid], axis=1)

  

# Ensure all columns have string type

OH_X_train.columns = OH_X_train.columns.astype(str)

OH_X_valid.columns = OH_X_valid.columns.astype(str)
```

We managed to get the error down to ~2000 from ~3000
