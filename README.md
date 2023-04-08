# Experiment-2--Implementation-of-Perceptron
## AIM:

To implement a perceptron for classification using Python

EQUIPMENTS REQUIRED:
Hardware – PCs
Anaconda – Python 3.7 Installation / Google Colab /Jupiter Notebook

RELATED THEORETICAL CONCEPT:
A Perceptron is a basic learning algorithm invented in 1959 by Frank Rosenblatt. It is meant to mimic the working logic of a biological neuron. The human brain is basically a collection of many interconnected neurons. Each one receives a set of inputs, applies some sort of computation on them and propagates the result to other neurons.
A Perceptron is an algorithm used for supervised learning of binary classifiers.Given a sample, the neuron classifies it by assigning a weight to its features. To accomplish this a Perceptron undergoes two phases: training and testing. During training phase weights are initialized to an arbitrary value. Perceptron is then asked to evaluate a sample and compare its decision with the actual class of the sample.If the algorithm chose the wrong class weights are adjusted to better match that particular sample. This process is repeated over and over to finely optimize the biases. After that, the algorithm is ready to be tested against a new set of completely unknown samples to evaluate if the trained model is general enough to cope with real-world samples.
The important Key points to be focused to implement a perceptron:
Models have to be trained with a high number of already classified samples. It is difficult to know a priori this number: a few dozen may be enough in very simple cases while in others thousands or more are needed.
Data is almost never perfect: a preprocessing phase has to take care of missing features, uncorrelated data and, as we are going to see soon, scaling.
Perceptron requires linearly separable samples to achieve convergence.
The math of Perceptron
If we represent samples as vectors of size n, where ‘n’ is the number of its features, a Perceptron can be modeled through the composition of two functions. The first one 
f(x) maps the input features  ‘x’  vector to a scalar value, shifted by a bias ‘b’

A threshold function, usually Heaviside or sign functions, maps the scalar value to a binary output:

Indeed if the neuron output is exactly zero it cannot be assumed that the sample belongs to the first sample since it lies on the boundary between the two classes. Nonetheless for the sake of simplicity,ignore this situation.


ALGORITHM:
Importing the libraries
Importing the dataset
Plot the data to verify the linear separable dataset and consider only two classes
Convert the data set to scale the data to uniform range by using Feature scaling

Split the dataset for training and testing
Define the input vector ‘X’ from the training dataset
Define the desired output vector ‘Y’ scaled to +1 or -1 for two classes C1 and C2
Assign Initial Weight vector ‘W’ as 0 as the dimension of ‘X’
Assign the learning rate
For ‘N ‘ iterations ,do the following:
        v(i) = w(i)*x(i)
         
        W (i+i)= W(i) + learning_rate*(y(i)-t(i))*x(i)
Plot the error for each iteration 
Print the accuracy


 PROGRAM:
