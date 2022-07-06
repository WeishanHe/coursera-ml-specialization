# Regression with Multiple Input Variables
## Multiple Linear Regression
#### Multiple features
![multiple_features_notation](images/multiple_features_notation.png)
![mlr_model](images/mlr_model.png)

#### Vectorization
neat and faster
![vectorization1](images/vectorization1.png)
![vectorization2](images/vectorization2.png)
![vectorization3](images/vectorization3.png)
#### Optional lab: Python, NumPy and vectorization
#### Gradient descent for multiple linear regression
![vctorized_gd1](images/vctorized_gd1.png)
![gd_mlr](images/gd_mlr.png)
![normal_eq](images/normal_eq.png)

#### Optional Lab: Multiple linear regression
## Gradient Descent in Practice
#### Feature scaling
A good model will assign small value to $w$ when the value of $x_i$ is large
![feature_parameter_scale](images/feature_parameter_scale.png)
It takes small change in $w_1$ to have a large impact on y given the range of value of $x_1$ is large and vise versa.
![feature_parameter_size](images/feature_parameter_size.png)
When the contour plot is skinny, gradient descent will bounce back and forth and therefore takes a long time to reach the minimum.
![feature_size_gd](images/feature_size_gd.png)
Feature scaling approach 1: max normalization
![feature_scaling_max_normalization](images/feature_scaling_max_normalization.png)
Feature scaling approach 2: mean normalization
![feature_scaling_mean_normalization](images/feature_scaling_mean_normalization.png)
Feature scaling approach 3: z-score normalization
![feature_scaling_zscore](images/feature_scaling_zscore.png)
When do we need to do feature scaling. There is no harm in doing feature scaling.
![feature_scaling](images/feature_scaling.png)
#### Checking gradient descent for convergence
- Learning curve: Adjust the learning rate. The number of iterations can varies a lot.
- Automatic convergence test: hard to choose an appropriate $\epsilon$ 
![check_convergence](images/check_convergence.png)

#### Choosing the learning rate
![choose_learning_rate](images/choose_learning_rate.png)
- Signs of problem: the learning curve fluctuate or keep increasing
- Potential problems, detection, and correction:
	- There is bugs in the code: test use a small enough $\alpha$ and see whether $J(\vec{w}, b)$  decrease on every iteration
	- Learning rate is too large: try a set of $\alpha$ for a handful of iterations and choose the $\alpha$ that seems to decrese the $J(\vec{w}, b)$ most rapidly.
![choose_learning_rate2](images/choose_learning_rate2.png)

#### Optional Lab: Feature scaling and learning rate
#### Feature engineering
![feature_engineering](images/feature_engineering.png)
#### Polynomial regression
- It is important to do feature scaling in polynomial regression
![polynomial_regression](images/polynomial_regression.png)

#### Optional Lab: Feature engineering and Polynomial regression
#### Optional Lab: Linear regression with scikit-learn
