<img src="https://miro.medium.com/max/968/1*F6SrJR7_s95r6oCF3ugMZw.png" alt="Logo">

## Article Link: https://medium.com/@7bn/neural-network-101-4a4383e7c7d0

# Neural Network 101

## What is Deep Learning?

This term was coined by an English Canadian computer scientist ***Dr.Geoffrey Everest Hinton in** 1995.* 

Deep Learning is an Artificial intelligence function which mimics the working of a human brain in processing and analyzing and processing data to create pattern which are used in decision making.

Deep Learning is a part of Machine learning in artificial intelligence that has network capable of learning from a unsupervised method using a unstructured and unlabeled data. These networks are known as deep learning networks or Neural networks

## **What is Neural Networks?**

Artificial Neural Networks or Neural network is the closest humans ever achieve to developing a artificial brain which can learn by it's own and it's a collection of nodes and neurons which further develops a complex structure which resembles to a human brain. 

As we know that Neuron is the basic building block of the human brain and the the neuron is responsible to transport signals received from the external stimulus and collection of neuron builds up the brain and which eventually takes the decision on responding to the stimulus, Perceptron is an analogous to Neuron, as Perceptron is also the building and elementary unit of a Neural Network. The term Perceptron is introduced by Frank Rosenblatt in 1957 according to whom, Perceptron is as single layered Neural Network with no hidden Layer. The collection of Perceptron is known as Neural Network.



## How Neural Network Works?



Let's consider above illustration as an example for Neural Network, this NN doesn't have any hidden layer. This process of having no or one hidden layer is known as Shallow Learning and when the number of hidden layers exceed two or more than two we use the term Deep Learning to describe the process.

Let's say we have three input parameters $x_1,x_2,x_3$ In the first step we assign random weights to the input variables i.e. $w_1, w_2, w_3$ then to calculate the output value $y$ we add the product of input parameters and weights, but we have to activate the nodes using various activation functions.

### What are Activation Functions?

the activation function of a node defines the output of that node given an input or set of inputs. A standard integrated circuit can be seen as a digital network of activation functions that can be ***"ON" (1) or "OFF" (0)***, depending on input. This is similar to the behavior of the linear perceptron in neural networks. 

**There are four most important activation functions:**

**Threshold or Binary Step Function :** The output is set at one of two levels, depending on whether the total input is greater than or less than some threshold value.



**Sigmoid:** The sigmoid function consists of 2 functions, logistic and tangential. The values of logistic function range from 0 and 1 and -1 to +1 for tangential function.



**Piecewise Linear or Rectified Linear Activation Function:**



**Hyperbolic Tangent Activation Function: tanh** is also like logistic sigmoid but better. The range of the tanh function is from (-1 to 1). tanh is also sigmoidal (s - shaped).



### Best practices while using Activation Functions:



- Use , ****but be careful with the learning rate and monitor the fraction of dead units.**ReLU** in hidden layer activation
- If **ReLU** is giving problems. Try Leaky ReLU, PReLU, Maxout. Do not use sigmoid
- **Normalize the data in order to achieve higher validation accuracy, and standardize if you need the results faster**
- The **sigmoid** and **hyperbolic tangent** activation functions cannot be used in networks with many layers due to the vanishing gradient problem.

After performing all the above steps we calculate the output $y$ and then we compare the value with actual value of $y'$ and then we check the difference between the actual value and calculated value by a function called Cost Function or Loss Function

$Cost Function =$ $1/2(y'-y)^2$

Then after getting the value of cost function the weights of all the inputs get optimized so that the value of Cost Function can reduced to as much as possible. Cost Function is inversely Proportional to the accuracy of the Neuron. After this the weights get recalibrated and again the cost function is calculated and this process repeats till the convergence criteria is met.

## Few Key Terms:

### What is Epoch?

One epoch completes when an entire dataset is passed forward and backward through the neural network only once.

### What is Backpropagation?

Back Propagation is a short for backward propagation errors. It is the practice of fine tuning the weight of the neural network based on the rate of error i.e. Loss/ Cost Function obtained in the previous epoch.
