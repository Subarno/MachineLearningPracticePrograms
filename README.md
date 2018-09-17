# A Machine Learning Walk-Through
This repository contains algorithms and techniques that are often used in machine learning problems implemented with minimal dependencies possible.
Requirements are python 3.5.3 (or above), numpy, matplotlib, and keras(only for LSTM and ConvNet).

In this repo we try to implement general machine learning algorithms and calculations for learning purpose. The modules implemented are described below. The codes used in this repo are inspired from various sources on the web.

### SVM ###
A Support Vector Machine (SVM) is a discriminative classifier formally defined by a separating hyperplane. In other words, given labeled training data (supervised learning), the algorithm outputs an optimal hyperplane which categorizes new examples. The calculations performed are based on this [link](https://github.com/MaviccPRP/svm/blob/master/svm-primal.ipynb).
<br>[CODE](svm.py)

### k-means Clustering ###
k-means clustering aims to partition n observations into k clusters in which each observation belongs to the cluster with the nearest mean, serving as a prototype of the cluster. This results in a partitioning of the data space into Voronoi cells. Lloyd's algorithm for k-means clustering is implemented over mnist dataset with varying k from 5 to 25.
<br>[CODE](kmeans.py)

### Logistic Regression ###
 Logistic regression is a generalized linear model that we can use to model or predict categorical outcome variables. In logistic regression, we’re essentially trying to find the weights that maximize the likelihood of producing our given data and use them to categorize the response variable. We implement a binary classifier in Logistic Regression model that classifies a toy data built on Gaussian distribution.
 <br>[CODE](logistic_reg.py)

### Linear Regression ###
 In statistics, linear regression is a linear approach for modeling the relationship between a scalar dependent variable y and one or more explanatory variables (or independent variables) denoted X. We implement a linear regression model over a toy dataset and compute the root mean sqaure error.
 <br>[CODE](linear_reg.py)

### Naive Bayesian Classifier ###
 It is a classification technique based on Bayes' Theorem with an assumption of independence among predictors. In simple terms, a Naive Bayes classifier assumes that the presence of a particular feature in a class is unrelated to the presence of any other feature. We implement a binary classifier in Naive Bayesian model that classifies over [pima-indians-diabetes dataset](https://archive.ics.uci.edu/ml/datasets/Pima+Indians+Diabetes) from UCI Machine learning repository.
 <br>[CODE](naive_bayes.py)

### Simplest Neural Network ###
 A neural network is a a computer system modelled on the human brain and nervous system. It is the simplest implementation with toy dataset that one could imagine. Lets begin my neural network journey with this!
 <br>[CODE](simple_nnet.py)

### Simple Convolutional Neural Network ###
 In machine learning, a convolutional neural network (CNN, or ConvNet) is a class of deep, feed-forward artificial neural network that have successfully been applied to analyzing visual imagery. [LeNet](http://yann.lecun.com/exdb/publis/pdf/lecun-98.pdf) is implemented using keras over [mnist](http://yann.lecun.com/exdb/mnist/) dataset. Its one of the simplest forms of ConvNet.
 (CONV-POOL-CONV-POOL-CONV-FC)
 <br>[CODE](mnist_cnn_lenet.py)

### Recurrent Neural Network ###
 A recurrent neural network (RNN) is a class of artificial neural network where connections between units form a directed cycle. This allows it to exhibit dynamic temporal behavior. Unlike feedforward neural networks, RNNs can use their internal memory to process arbitrary sequences of inputs. We develop a word level Vanilla RNN for predicting sequences of text.
 <br>[CODE](min_word_rnn.py)

### LSTM Network ###
  Long Short Term Memory networks – usually just called “LSTMs” – are a special kind of RNN, capable of learning long-term dependencies. They were introduced by Hochreiter & Schmidhuber (1997), and were refined and popularized by many people in following work.1 They work tremendously well on a large variety of problems, and are now widely used. All recurrent neural networks have the form of a chain of repeating modules of neural network. In standard RNNs, this repeating module will have a very simple structure, such as a single tanh layer. We implement LSTM network with keras for a regression problem on [International airline passengers dataset](https://datamarket.com/data/set/22u3/international-airline-passengers-monthly-totals-in-thousands-jan-49-dec-60#!ds=22u3&display=line), for estimating the number of passengers next month.
  <br>[CODE](lstm.py)
