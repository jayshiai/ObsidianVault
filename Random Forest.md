The random forest uses many decision trees, and it makes a prediction by averaging the predictions of each component tree. It generally has much better predictive accuracy than a single decision tree and it works well with default parameters.

Let's use `Random Forest Regressor` from sklearn to see if it gives us better results : 

```python

from sklearn.ensemble import RandomForestRegressor

forest_model = RandomForestRegressor(random_state=1)
forest_model.fit(train_X, train_y)
preds = forest_model.predict(val_X)
print(mean_absolute_error(val_y, preds))

```

Error = 
```python
4019.7890813008135
```

That's improvement over our last result of `5399`.

Be we can still do better. Lets see how in [[Intermediate Machine Learning]]