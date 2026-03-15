
## Hidden Layer Network
There is a very specific function that one could refer to as the 1-hidden-layer neural network. It is a function of the form:
$$f_\theta(x) = W_2 \sigma(W_1 x + b_1) + b_2$$
where $\sigma$ is a non-linear function, such as the ReLU function. When you pick small dimensions, this is effectively the simplest valid neural network function. If $\sigma$ were linear, then this would just be a linear function, and we know that linear functions are not very powerful. The non-linearity is what gives the neural network its power. In particular, the non-linearity is what allows networks to approximate arbitrary functions. 

Somehow in this definition, we have inputs $x$, and parameters $\theta = (W_1, b_1, W_2, b_2)$. Inputs are the data we will process and parameters are what we will learn in training. This is a conceptual definition: practically, these are all free variables to start with. However, $x$ will be given by the source of data, and $\theta$ will initially be selected randomly, then learned via a training process. 

## Parametrised Functions
One could say that a neural network is a parametrised function with universal approximation. This would be a more general definition, but it could include other objects that are generally not considered to be neural networks. For example, decision trees are also universal approximators. Moreover, there are many neural networks that have not yet been proven to be universal approximators, but are still broadly considered neural networks. 

## Conditional Probability Distributions
Often in papers, neural networks are defined as conditional probability distributions. This is because they are often used to model the probability of an output given an input. For example, in classification tasks, a neural network might output a probability distribution over classes given an input image.


## Theorems of Neural Networks 
In this section, we will prove some theorems about neural networks. 

- Universal Approximation Theorem 
- No Free Lunch Theorem
- Lottery Ticket Hypothesis
- Neural Tangent Kernel
- Double Descent Phenomenon

All of these theorems are interesting and will be explained as simply as I can. 