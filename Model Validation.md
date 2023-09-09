#documentation #Machine_Learning #sklearn 
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

That's because we used the model to predict values of data it was trained on instead of new data. Which is like creating Math's paper made up of problems students have already seen instead of asking new questions.

But how do we bring in new data, since we already used all our data to train our model?

The most straightforward way to do this is to exclude some data from the model-building process, and then use those to test the model's accuracy on data it hasn't seen before. This data is called **validation data**.

## Let's code it.

Again sklearn come with a prebuilt function called `train_test_split`.

```python
from sklearn.model_selection import train_test_split

train_X, val_X, train_y, val_y = train_test_split(X, y, random_state = 0)
```

Now retrain the model one the training data and the use validation data to make predictions and calculate its error.

```python
model.fit(train_X,train_y)

val_predictions = model.predict(val_X)

mean_absolute_error(val_y, val_predictions)
```

Output :

```python
5399.359756097561
```


## Woah!

Our first MAE was **5.4570** while its **5399** right now. That's _1000x_ more!

This is the difference between a model that is almost exactly right, and one that is unusable for most practical purposes. As a point of reference, the average car price in the validation data is 18425 dollars. So the error in new data is about a quarter of the average car price.

Let's try a new model called [[Random Forest]] to see if we can get better results.