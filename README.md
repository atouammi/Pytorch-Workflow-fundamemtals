# Pytorch-Workflow-fundamemtals

## What we cover in this repos?

- ### Data (preparation and loading)
- ### Buil model
- ### fitting the model to data( training)
- ### making predictions and evaluatung a model(inference)
- ### Saving model and loading a mode
- ### puting it all together


 ## 1.  Data (preparation and loading)

Data can be almost anything in machine leraning
- Excel spreasheet
- Images of any king
- video
- audio
- NDA
- Text

Machine learning is game of two parts:

1. Get data into meanfull numerical representation
2. Build a model to learn pattern in that numerical representation




## 2. Build Model

### Our first PyTorch model
This is very exciting...let's do it!
Because we're going to be building classes throughout the couse, I'd recommend getting familiar with OOP in Python, to do so you can
use the following resource from Real Python : https://realpython.com/python3-object-oriented-programming/
nn.module documentations : https://pytorch.org/docs/stable/generated/torch.nn.Module.html
What our model does:
Start with random values (weight and bias)
Look at training data and adjust the random values to better represent (or get closer to) the ideal values (the weight & bias) values
we used to create the data.
How does it do so?
Through two main algorithms
1. `Gradient Descent`
2. `Backpropagation`



## 3. Train model
The whole idea of training is for a model to moce from some unkown parameters (these may be random) to some known parameters.
Or in other words form a poor representation of the dat to a better representation of the data.
One way to measure how poor or haow wrong your models predictions are is to use a loss function.
Note: loss function may also be called cost functionor criterion in different areas. For our case, we're going to refer to it as a loss
function.
Things we need to train:
- Loss function:  
A function to measure how wrong your model's predictions are to the ideal outputs, lower is better. -
https://pytorch.org/docs/stable/nn.html#loss-functions
- Optimizer:  
Takes into account the loss of model and adjusts the model's parameters (e.g. weight & bias in our case) ot improve the
loss function. - https://pytorch.org/docs/stable/optim.html
- Inside the optimizer you'll often have to set two parameters:  


    - params - the model parameters you'd like to optimize, for example params = model_0.parameter()
    - lr (Learning rate) - the learning rate is a hyperparameter that defines how big/small the optimizer changes the parameters
    with each step (a small lr result in small changes, a large lr result in large changes)
    And specifically for PyTorch, we need:
    - A training loop
    - A testing loop




