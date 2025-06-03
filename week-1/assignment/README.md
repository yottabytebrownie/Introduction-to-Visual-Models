# Tensorflow library
It is an open-source machine learning library developed by Google. It provides tools and functionalities to build, train and deploy machine learning models.
Have a look through [this](https://www.tensorflow.org/tutorials/quickstart/beginner) to undestand the basics of tensorflow. 
[Overfitting and underfitting](https://www.tensorflow.org/tutorials/keras/overfit_and_underfit)
[Saving and loading models](https://www.tensorflow.org/tutorials/keras/save_and_load)
# The assignment
## Activations
[Activation functions](https://www.geeksforgeeks.org/types-of-activation-function-in-ann/) are mathematical equations used in artificial neural networks to determine the output of a node (or neuron), given an input or set of inputs. They help introduce non-linearity into the model, enabling the network to learn complex patterns in data.
Without them, neural networks would behave like simple linear models.
Some common activation functions include 
* Sigmoid
* identity
* ReLU
* hyperbolic tangent

We use the libraries `numpy` and `math`.
`import numpy as np`
`import math`

We define a class called `Activations`. These activation functions are scalar operations; they shouldn't change the shape of the input.

`class Activation(object):
    def __init__(self):
        self.state = None
    def __call__(self, x):
        return self.forward(x)
    def forward(self, x):
        raise NotImplemented
    def derivative(self):
        raise NotImplemented`

`Identity` activation function has been implemented for you:

`class Identity(Activation):
    def __init__(self):
        super(Identity, self).__init__()
    def forward(self, x):
        self.state = x
        return x
    def derivative(self):
        return 1.0`

Now, **you** must implement the activation functions: Sigmoid, tanh, ReLU.
Import the libraries and define the class `Activation` as described above (don't make any changes!), afterwhich you may define the activation function classes.
For an example of how they look, here is Sigmoidal activation function:

`class Sigmoid(Activation):
    # Do not change the function signatures 
    def __init__(self):
        super(Sigmoid, self).__init__()
    def forward(self, x):
        # What do we need to store before returning???
        raise NotImplemented
    def derivative(self):
        # What do we need to store before returning??? 
        raise NotImplemented`

This exercise tests your implementation of `forward` and `derivative` class methods. 

**Remove `raise NotImplemented` in your code.**

## Loss function
A [loss function](https://www.geeksforgeeks.org/loss-functions-in-deep-learning/) is a tool that tells us how bad our model's predictions are. It tells the model how far off its answers are, so it can learn and improve. In part 2 of the assignment, you have a base class called `Criterion`. The `SoftmaxCrossEntropy` class computes the loss and gradient for classification tasks in neural networks.

## Linear Layer
A linear layer is a basic building block in a neural network. It takes some numbers in (inputs), multiplies them by weights, adds a bias, and gives new numbers out.

## Multi-layered perceptron (MLP)
A Multilayered Perceptron is a type of neural network made up of layers of linear layers + activations, stacked together to learn complex patterns. Its structure is as follows:
* Input layer – where the data enters (e.g. image pixels, numbers).
* Hidden layers – one or more layers that process the data.
* Output layer – gives the final prediction (e.g. class label or number).
