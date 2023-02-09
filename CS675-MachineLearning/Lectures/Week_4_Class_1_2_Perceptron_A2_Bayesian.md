## Class 2:
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


### Bayes Theorem

Posterior ~ likelihood * Prior
P(A|B) ~ P(B|A) P(A)

Hypothesis - the model we have chose. we assuume we have a linear model 
Bayesian Learning - Posterior probability P(h|D) = P(D|h)*P(h)/P(D)       [D = Dataset, h=hypothesis]

#### Choosing Hypothesis
hMAP (Maximum a Posterori)
MLE = Max likelihood estimation



## Class 2:
#### Bayes Theorem
- P(A|B) = P(B|A)P(A)/P(B) See the picture for details in slides
- Posterior portional to likelihood * Prior 
- P(B) == P(D) some information about data - constant
- argmax - find and h which makes the value of P max - hMAP are the w values
- If we drop hypothesis we find likelihood and maximize it.

Example 1: Bernouli Trials

- Faulty lighbulbs
- Use argmax to get best Probability
- use symbolab and set zero and get the solution.
- P<sub>best</sub> = a/(a+b)

#### MAP with logistic regression
- to minimize after log minus term to make it small. Regularization
- Smoother
- differentiate, zero and gradient decent
- 1/sigma<sup>2</sup> regularizer
- sigma is the hyperparameter
- choose sigma because we assume hypothesis space gaussian/normal distribution.

#### Summary: Learning as Loss minimization
- Setup
    - Examples of x, unkown D
    -  Hidden oracle f label
    - find hypothesis
- The ideal situation
    - function L that penalizes bad hypothesis
    -  pick a funtion that minmizes. empirical loss.
    - for regularizer we have seen in last section.
    - Learning with linear classsifier
    - quuadratic because 1 unknown.
    - Theoritical explanation needed in qual.






