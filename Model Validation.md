
To check the validity of model, we compare the predicted values with the actual values and calculate the `error`. Lower the error, better the model.

Many `metrics` can be used for calculating this error. For now we'll use `Mean Absolute Error (MAE)` .


sklearn come with many metrics already built into it and ready to use. Let's import MAE.

```python
from sklearn.metrics import mean_absolute_error
```

Now, we'll calculate the MAE.

```python
predicted_prices = model.predict(X)

mean_absolute_error(y, predicted_prices)
```
Output = 
```python
5.475064816226933
```

That is a very low error. Which is good. But should you be celebrating?

**NO!**

That's be