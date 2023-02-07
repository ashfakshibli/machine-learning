### Logistic Regression

#### Linear separability
- Separate features with a hyperplane (separates the space, at least 1 less plane than the space) in n dimension
- Overfitting

#### Better classifier
- find a line which minimizes misclassification
- in regression we used many parameters. (a curve)

#### Perceptron Algorithm
##### Preview
- Linear classifiers. sgn function is plugged in with essentially a DOT product.
- sign function (non differentiable, discrete, classifies directly): [-1, 1] similar to sigmoid fuunction (differentiable, continuous)
- perceptron uses sign function. Also serves as a activation function.
- w = weights/model parameters, give us a vector. Only can rotate at origin. For shifting we need bias.
- dot produuct min bias = zero
##### Algo
- sequence training x1, y1 .... xn, yn
- initialize w0  = 0
- for each example predict y
- if error/misclassification update w (perceptron update)

1. Convergence
2. Voting and Averaging
3. Margin of data, perceptron





