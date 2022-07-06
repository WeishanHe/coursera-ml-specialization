# Regression with Multiple Input Variables
## Multiple Linear Regression
#### Multiple features
<img src="images/multiple_features_notation.png" with="250" height="250">
<img src="images/mlr_model.png" with="250" height="250">

#### Vectorization
neat and faster
<img src="images/vectorization1.png" with="250" height="250">
<img src="images/vectorization2.png" with="250" height="250">
<img src="images/vectorization3.png" with="250" height="250">

#### Optional lab: Python, NumPy and vectorization
#### Gradient descent for multiple linear regression
<img src="images/vctorized_gd1.png" with="250" height="250">
<img src="images/gd_mlr.png" with="250" height="250">
<img src="images/normal_eq.png" with="250" height="250">

#### Optional Lab: Multiple linear regression
## Gradient Descent in Practice
#### Feature scaling
A good model will assign small value to $w$ when the value of $x_i$ is large
<img src="images/feature_parameter_scale.png" with="250" height="250">

It takes small change in $w_1$ to have a large impact on y given the range of value of $x_1$ is large and vise versa.
<img src="images/feature_parameter_size.png" with="250" height="250">

When the contour plot is skinny, gradient descent will bounce back and forth and therefore takes a long time to reach the minimum.
<img src="images/feature_size_gd.png" with="250" height="250">

Feature scaling approach 1: max normalization
<img src="images/feature_scaling_max_normalization.png" with="250" height="250">

Feature scaling approach 2: mean normalization
<img src="images/feature_scaling_mean_normalization.png" with="250" height="250">

Feature scaling approach 3: z-score normalization
<img src="images/feature_scaling_zscore.png" with="250" height="250">

When do we need to do feature scaling. There is no harm in doing feature scaling.

<img src="images/feature_scaling.png" with="250" height="250">

#### Checking gradient descent for convergence
- Learning curve: Adjust the learning rate. The number of iterations can varies a lot.
- Automatic convergence test: hard to choose an appropriate $\epsilon$ 
<img src="images/check_convergence.png" with="250" height="250">

#### Choosing the learning rate
<img src="images/choose_learning_rate.png" with="250" height="250">

- Signs of problem: the learning curve fluctuate or keep increasing
- Potential problems, detection, and correction:
	- There is bugs in the code: test use a small enough $\alpha$ and see whether $J(\vec{w}, b)$  decrease on every iteration
	- Learning rate is too large: try a set of $\alpha$ for a handful of iterations and choose the $\alpha$ that seems to decrese the $J(\vec{w}, b)$ most rapidly.
<img src="images/choose_learning_rate2.png" with="250" height="250">

#### Optional Lab: Feature scaling and learning rate
#### Feature engineering
<img src="images/feature_engineering.png" with="250" height="250">

#### Polynomial regression
- It is important to do feature scaling in polynomial regression
<img src="images/polynomial_regression.png" with="250" height="250">

#### Optional Lab: Feature engineering and Polynomial regression
#### Optional Lab: Linear regression with scikit-learn
