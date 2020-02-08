### PCA- Principal Component Analysis

Principal component analysis is a technique for feature extraction — so it combines our input variables in a specific way, then we can drop the “least important” variables while still retaining the most valuable parts of all of the variables! As an added benefit, each of the “new” variables after PCA are all independent of one another.<br>

When to use: when you want to ensure variables are independent of one another, When you have lots of variables, overfitting could be a problem in that case. You want to reduce the dimension of your feature space, so that you have fewer relationships between features to consider and you are less likely to fit overfit your model.<br>

How to reduce dimension: Feature elimination: we might drop all the variables except the ones we think will predict target variable best. There could be information loss. <br>
Feature Extraction: New independent variables which are a combination of old independent variables. Order the new variables in a specific way by how well they predict our dependent variable. Therefore we know which variable is most impt. <br>
Eigenvectors represent directions, eigenvalues represent magnitude and relation with other variables. <br>
