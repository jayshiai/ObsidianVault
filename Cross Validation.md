#documentation #sklearn #Machine_Learning 
![[Pasted image 20230909162920.png]]

```python
from sklearn.model_selection import cross_val_score

scores = -1 * cross_val_score(my_pipeline, X, y,

                              cv=10,

                              scoring='neg_mean_absolute_error')

  

print("MAE scores:\n", scores)

print(scores.mean())
```
