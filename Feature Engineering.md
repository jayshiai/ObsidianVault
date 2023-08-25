The goal of feature engineering is simply to make your data better suited to the problem. 

We can use Feature Engineering to:
- improve model's predictive power
- reduce computational or data needs
- improve interpretability of the data

For example: say you were trying to predict the Price of square plots of land from the Length of one side. Fitting a linear model directly to Length gives poor results: the relationship is not linear.
![[Pasted image 20230825104023.png]]


If we square the Length feature to get 'Area', however, we create a linear relationship. 

![[Pasted image 20230825104126.png]]

Adding Area to the feature set means this linear model can now fit a parabola. Squaring a feature, in other words, gave the linear model the ability to fit squared features.
