---
layout: post
title:  "I scream DataScience"
categories: jekyll update
date:   2020-04-01 10:51:47 +0530
img: e.jpg
---

Data science is an inter-disciplinary field that uses scientific methods, processes, algorithms and systems to extract knowledge and insights from many structural and unstructured data.


##### [Markdown link of this same page rendered by Github ] <a href="https://github.com/IJyotir/myProfile/blob/gh-pages/_posts/2015-04-24-i-scream.markdown" class="btn btn-primary btn-xs">MD LINK</a>

# Feed Forward Neural Network :
#### Date 04-Feb-2020
- Understanding the buzz words in simple English :)
	1.  Logistic Regression transition to FNN
	2.  Non-Linearity
	3.  Activation functions
	4.  FNN in Pytorch
	5.  Live coding and line by line explanation of the Neural Network .
	6.  Writing the code in CPU and GPU
	7.  Understanding Hidden layers
	8.  Understanding Hidden Neurons
	9.  Understanding Readout Layers
	10.  Weights and Biases
	11.  Maths behind the code .
	12.  Each Layer input output .

- Details and Code in Pytorch :[Creating a Feed Forward NN using Logistic and Linear Regression : ](https://github.com/ijbo/ML_Theory/blob/master/Pytorch/Feed_Forward_NN.ipynb)
- This code can be run on GCP : [Colab Notebook](https://github.com/ijbo/ML_Theory/blob/master/Pytorch/FeedForwardNN_colabs.ipynb)

# Logistic Regression :
#### Date 04-Feb-2020
- Code in Pytorch **[Logistic Regression : Click to open Notebook](https://github.com/ijbo/ML_Theory/blob/master/Pytorch/Logistic_Regression.ipynb)**
- This code can be run on GCP : **[Colab Notebook](https://github.com/ijbo/ML_Theory/blob/master/Pytorch/Logistic_regression_colabs.ipynb)**
- Logistic Regression :
	1.  What is used for
	2.  Why it is used in Deep Learning
	3.  How it is used in DL
	4.  Loss function in Linear regression
	5.  Gradient Descent in Linear Regression
	6.  Back Propagation in DL
	7.  Multiclass and Multilabel.	
	8.  Softmax and Sigmoid Function .
	9.  Cross Entropy loss function

# Linear Regression :
#### Date 04-Feb-2020
- Code in Pytorch **[Linear regression : Click to open Notebook](https://github.com/ijbo/ML_Theory/blob/master/Pytorch/Linear_Regression.ipynb)**
- The Notebook contains a high level understanding of the Linear regression and how to make it work with Pytorch library. 
- This code can be run on GCP : **[Colab Notebook](https://github.com/ijbo/ML_Theory/blob/master/Pytorch/Linear_Regression_colabs.ipynb)**
- Understand the  code Steps:
	- Step 1: Load Dataset
	- Step 2: Make Dataset Iterable
	- Step 3: Create Model Class
	- Step 4: Instantiate Model Class
	- Step 5: Instantiate Loss Class
	- Step 6: Instantiate Optimizer Class
	- Step 7: Train Model 

# Gradients :
#### Date 04-Feb-2020

### 1.  What is Gradients ?
- Gradients are slope of a Tangent , in past we have studied Slope of a line. 
- Slope of a line is Rise/Run that is the change in Y divided by the change in X.
- Since the loss functions are not a straight line we need to find slope of a Tangent in that loss function w.r.t change in the weights or parameters.
- To do this we use Calculus and the Maths of it is covered below.

### 2.  The Maths behind Gradients
- Calculus is also called as infinitesimal **calculus** or "the **calculus** of infinitesimals" 
- In Latin, Calculus means Pebble. Mathematics was done using Pebble or small stones in past.
- What Calculus isto, as Geometry is about shapes, Algebra is about Relationships , Probability is about Predictions or chance , **Calculus** is about all the things that change.
-  17th century both Isaac Newton and Gottfried Wilhelm Leibniz started working on a problem and invented Calculus.
- Isaac Newton was trying to find how Gravity changes over distance, the equation tells us gravity is inversely proportional to distance . 
- $\large Gravity \propto  \frac {\large 1}{\large Distance}$ : Latex is not supported on the blog us can open the Markdown link.
- If you plot Gravity and Distance it is a curve and not a straight line, so finding slope of a curve was not possible using the avaliable mathematics.
- Here Newton was trying to calculate the gradient of a Tangent and not the gradient of a Secant.
- **[Calculus Video 1 links ](https://www.youtube.com/watch?v=tt2DGYOi3hc)**
- **[Calculus Video 2 links](https://www.youtube.com/watch?v=50Bda5VKbqA)**
- These two Videos are sufficient to explain , why do we need calculus to find Gradient of a Loss function.

### 3.  Why Gradients are used in ML?
- In Machine Learning We have the find the best possible Hypothesis which provides the least amount of loss .  
- **Hypothesis**: y_pred = mx + b
- **Parameters** : m (coefficient,slope, gradient , weights) , b (Bias , intercept)
- **Actual function** : y_actual= 2x + 1
- **Parameters** : 2 (coefficient,slope, gradient , weights) , 1 (Bias , intercept)
- **Minimize** : the distance y_pred and y_actual
-  Initially we start with some random values of the Parameters in the Hypothesis function.
- Then we find the Loss and try to Minimize it , the process of Minimizing the loss is done by Calculating the Gradient and Back-propagation.

### 4.  How they help to reduce the loss function ?
- Gradient gives the change in the Loss w.r.t the change in the Coefficients.
- The Gradient has two elements a Sign (+ve or -ve) and a Value. 
- The Sign tells us the slope is Positive or slope is Negative and the direction of the minima of the loss function.
- The Value tells us the how much is the Slope.
- The Parameters which we have initialized [at the start while creating a NN] with some random value we update it with the change times the Learning rate.
- Learning Rate scales the change(slope or Gradient) so that we don't increase or Decrease the parameters by too much.
- This way we keep repeating this step to minimize the loss and better the Hypothesis function.

### 5.  What is Forward propagation ?
- **[Solving XOR with Neural Net : click here ](https://www.youtube.com/watch?v=kNPGXgzxoHw&t=2s)**
- Here we understand how a simple Neural Net is constructed .
- Forward Propagation means moving from the start to the end of the network and calculate the loss.

### 6.  What is Back-propagation ?
- In Back-Propagation , we reduce the loss and update the parameters using Gradients and Chain Rule 
- This process of updating is also called as Optimizing and further we will read about the optimizes in details. 
- There are tuning done to the optimizer to improve on the speed to find the global minima of the loss function.

### 7.  The Chain rule of derivation .
- Chain Rule of Derivation helps to differentiate a function.
- Lets say a function f(x) = Ax+B and f(y)= C(f(x))+D , now to find the derivative of f(y) wrt to x, we need to find derivative of f(x) wrt to x .
- **[Chain rule in Back-propagation link ](https://www.youtube.com/watch?v=0e0z28wAWfg&t=659s)**

# Pytorch Fundamentals : 
#### Date 31-Jan-2020

**[Pytorch Fundamental : click to open Notebook ](https://github.com/ijbo/ML_Theory/blob/master/Pytorch/Pytorch_Fundatmentals.ipynb)**
- In this Fundamental Notebook I try to cover Numpy and Pytorch basics one need to start Pytorch coding .
- This Covers Topics like :
    1. Creating a Matrix.
    2. Create Matrices with Default values
    3. Seed for Reproduce
    4. Numpy to Torch Bridge
    5. Torch Tensor to Numpy
    6. Tensor Resize
    7. Element wise Operations
    8. Tensor Mean
    9. Variables and Gradients
    10. GPU-CPU toggling 

# Reasons to Learn Pytorch : 
#### Date 31-Jan-2020

(There is a link with the bold points) 
1. **[Tutorial](https://pytorch.org/tutorials/)** : The tutorial of Pytorch covers a lot of basics to Build a Deep Neural Net. Very easy to start development with pytorch since it  is very similar to Python.
2. **[Image](https://pytorch.org/tutorials/#image)**: Basic Examples on building Deep Neural nets and GAN's.
3. **[Audio](https://pytorch.org/tutorials/#audio)**: Lets you handle Audio files and provides api's for Machine Learning . 
4. **[Text](https://pytorch.org/tutorials/#text)**:  NLP using RNN and LSTM.
5. **[Why Pytorch](https://www.fast.ai/2017/09/08/introducing-pytorch-for-fastai/)** : This Link Provide one of the best Machine Learning courses using Pytorch.
6. Many Companies are adopting Pytorch 
-  [`Microsoft`](https://twitter.com/jeremyphoward/status/1182444543574044677?lang=en)
-  [`OpenAI`](https://twitter.com/OpenAI/status/1222927584033247232)
7. **[Comparisions between Pytorch and TF](https://builtin.com/data-science/pytorch-vs-tensorflow)**
