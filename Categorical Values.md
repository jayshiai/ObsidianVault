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


