
# Track Proposal 

## Title: Essential Maths for Data Science and Machine Learning 

### Introduction and Motivation

Data Science offers an immense range of possibilities for answering business questions in data driven industries. Some of the most popular methodologies in the field of data science are built around design and implementation of Machine Learning (ML) models for solving analytical business problems. A fundamental mathematical understanding of these models goes a long way towards bridging the gap between theory and practice in analytical environments. It also helps aspiring data scientists develop a strong intuitive thinking around ML model development and evaluation stages, where programming code is often written directly following some mathematical intuition. 

The essential mathematical concepts required for machine learning can be broadly grouped into five areas. These are highlighted along with their primary application areas in data science and ML below:

* **Linear algebra and matrix manipulation** is considered the most important area for developing statistical/neural ML algorithms and dimensionality reduction techniques. Advanced machine learning techniques including NLP and Computer Vision employ linear algebra heavily to deal with analyzing unstructured real world data. 

* **Optimization techniques** are integral part of most ML models. These are used for loss definition and loss minimization during model training stages. 

* **Multivariate calculus** deals with the differentiation and integration of functions involving multiple variables in order to determine the influence of model input on the output. Gradient descent and other such techniques are commonly used for approximating gradient functions in predictive modelling .

* **Probability theory and Bayesian statistics** aid the development and optimization of predictive models with Bayesian inferencing. Bayesian approach allows the application of probabilities to statistical models which forms the basis of predictive modelling techniques. Bayesian inferencing is heavily used in a number of statistical machine models as well as deep neural networks.  

* **Information theory** is used towards building logical and tree based models using the notion of information gain. This theory is applied in some of the most popular machine learning approaches including random forests and gradient boosting. The popular cross entropy function is deep learning also has its foundations in information theory.  

This track offers a combination of 7 courses aimed at providing learners with the essential mathematical vocabulary, concepts and skills necessary to get up and running in data science practice. The track is by no means an exhaustive maths curriculum. As highlighted above, it attempts to identify core topics from each of the listed areas. Special care has been taken to ensure that each mathematical idea gets related to some common practice in data science, to allow learners better relate theory to practice.   

### Track Pre-requisites

This track expects learners to have basic understanding of school level mathematics and some programming experience with Python and key libraries. Knowledge of a typical data science process and some applications domains may also come in handy for understanding wider applications of these skills. The course assumes no prior knowledge or experience of machine learning and modelling approaches. 

### Tools

All the courses included in the track use Python programming environment to code the core mathematical concepts. Numpy and SciPy scientific libraries have been used to simplify complex mathematical calculations and allow learners to focus more on developing an strong theoretical understanding of the concepts. Learners are neither required nor advised to use any machine learning library to fulfil the accompanying tasks.  

### Objectives: 

After successful completion of the proposed track, learners will be able to:


* Demonstrate a strong understanding of basic mathematical principles behind modelling practices commonly employed within data driven companies.

* Explain machine learning as a field that intersects statistical, probabilistic, computational and algorithmic aspects of intelligent models.

* Create simple yet scalable machine learning models in Python, Numpy and Scipy using core mathematical principles. 

* Demonstrate a competitive edge over peer data scientists with mathematical skills highly regarded by employers. 



## Course 1: Computational Thinking and Problem Solving in Python 

### Pre-requisites: 
* "Introduction to Python" by Filip Schouwenaars

### Introuction
This course details the fundamental concepts and systematic approaches towards computational problem solving, including problem decomposition, data abstraction, optimization and generalisation. Many business problems in data driven industries can be solved using computational approaches and hence understanding of basic computational problem solving techniques will provide you with strong foundation to deal with real world problems. You will learn fundamentals of building computational algorithms and implement a simple search algorithm in Python. The course also highlights the role of optimization in algorithmic problem solving with basic linear optimization techniques. This course is aimed at learners with some prior programming experience in Python. 

### Objectives:
Learners will be able to:

* Explain and differentiate between traditional computer programs and computational algorithms for analytical problem solving.
* Develop and describe a simple binary search algorithm using problem decomposition techniques in Python. 
* Create a simple experiment in Python to run linear optimization in order to minimize/maximize a given function. 

## Course 2: A Linear Algebraic View of Regression Analysis

### Pre-requisites: 
* "Introduction to Python" by Filip Schouwenaars

### Introduction
In this course, you will learn the fundamentals of linear algebra, the branch of maths that powers most machine learning algorithms. You will learn to use vectors and matrices as key algebra entities for framing real world problems in a computational domain. This course will provide a deeper understanding of how linear regression operates "under the hood", and equip learners with skills heavily employed in advanced machine learning approaches including computer vision, NLP and deep learning. Learners are expected to have some basic knowledge of Python programming, importing and using Numpy library and basic data types. 

### Objectives
Learners will be able to:
* Describe the roles of vectors, matrices and related algebraic operations for framing and solving analytical problems as systems of linear equations. 
* Describe and solve a simple regression problem using matrix algebra and Python programming, in order to fit a linear function to the given data.
* Apply Ordinary Least Squares (OLS) to estimate the parameters that optimally define the regression parameters. 

## Course 3: Matrix Decomposition Techniques for Machine Learning


### Pre-requisites
* "Introduction to Python" by Filip Schouwenaars
* "A Linear Algebraic View of Regression Analysis"

### Introduction

This course will teach you how to deal with the enormous challenges of processing "Big Data" in a fast and computationally efficient manner using various matrix decomposition techniques. The course provides an introduction and general use cases for matrix decomposition. You will learn to use LU and Cholesky decomposition techniques for solving challenging linear systems. The course will also focus on advance decomposition techniques: Eigen Decomposition and Singular Value Decomposition (SVD) for dimensionality reduction, data compression and building recommender systems. Learners are expected to have a basic knowledge of Python programming environment and Numpy, SciPy libraries and be familiar with basic matrix algebra principles and operations for matric manipulation. 


### Objectives
Learners will be able to:
* Explain a rationale for matrix decomposition and differentiate between different matrix decomposition techniques.
* Implement Principle Component Analysis (PCA) using Eigen decomposition for dimensionality reduction and data compression using Python and Numpy. 
* Implement and evaluate a simple recommender system using Singular Value Decomposition (SVD) in Python and SciPy.


## Course 4: Multivariate Calculus for Machine Learning 
### Pre-requisites
* "Introduction to Python" by Filip Schouwenaars
* "Computational Thinking and Problem Solving in Python"

### Introduction
This course offers an introduction to the multivariate calculus, a mathematical approach required to build many common machine learning algorithms. Most real world dataset are multivariate in nature and you will most likely use multivariate calculus to see how different variables play different roles in predicting the output. In this course, you will get an introduction to derivatives and how these are generalized to real values functions. You will also learn how gradient descent, a common optimization technique uses multivariate calculus to train a number of machine learning models. Learners are expected to have some experience of Python programming environment and using Numpy library and fundamentals of computational thinking and optimization aproaches. 

### Objectives
Learners will be able to:
* Explain the mathematical intuition behind derivation for calculating instantenous rate of change of a function. 
* Apply derivation rules and create a function to calculate the gradient of a function in Python and Numpy.
* Explain and apply the gradient descent algorithm to a multivariate dataset.

## Course 5: Similarity Measures in Data Analysis

### Pre-requisites
* "Introduction to Python" by Filip Schouwenaars

### Introduction
In this course, you will learn how to check similarity between data items by using different distance metrics. Similarity in data science generally dictates how similar two data objects are. You will be introduced with a number of similarity measures along with their use cases. You will set up simple experiments to compare different measures visually. You will also learn how to use euclidean distance and Pythagorus theorem to build a simple model to identify neighbors (i.e. similar data elements) of a given data element. You will finally take this architecture and build an unsupervised predictive model by ranking and selecting top neighbors. Learners are expected to have some programming experience in Python, Numpy and MatplotLib along with an understanding of basic data structures including lists and dictionaries. 


### Objectives
Learners will be able to: 

* Compare and contrast commonly used distance measures in terms of their use cases and implement these in Python, Numpy and MatplotLib.
    * Eucledian distance, Manhattan distance, Spearman correlation distance and Mahalanobis distance
* Create a distance based grouping algorithm by employing Pythagorean theorem to group together similar data items as "neighbors".  
* Build and evaluate a K-Nearest Neighbors (KNN) architecture by modifying the algorithm to rank and select a given number of top neighbors.

## Course 6: Information Theory and Decision Trees

### Pre-requisites
* "Introduction to Python" by Filip Schouwenaars
* "Computational Thinking and Problem Solving in Python"

### Introduction
This course covers basic Information theoretic principles used in implementing tree-based algorithms for regression or classification tasks. The course provides a deep dive into minimizing decision uncertainty using Shannon's Entropy and Information Gain approaches. Information theoretic models build their analytical approach using informational measures and allow modelling to be domain and data agnostic. Such Informational measures free you from typical machine learning assumptions, thus hugely simplifying the modelling process. In this course, you will write code to define optimal splitting in a tree structure for solving classification problems. The course is aimed at learners having knowledge of Python programming, NumPy and a basic understanding of monotonically increasing/decreasing logarithmic functions. 

### Objectives

Learners will be able to:
* Explain and implement Shannon's Entropy and Information Gain measures in Python and Numpy. 
* Build a function in Python to calculate information gain for identifying an optimal split in a decision tree algorithm.
* Implement complete ID3 tree classification algorithm for defining the decision boundary in a typical classification problem. 

## Course 7: Introduction to Bayesian Inferencing

### Pre-requisites
* "Introduction to Python" by Filip Schouwenaars
* "Computational Thinking and Problem Solving in Python"

### Introduction
This course will introduce you to Bayes theorem and conditional probabilities that form the basis of predictive modelling with statistical machine learning algorithm. Bayesian approach allows you to integrate probabalistic into statistical approaches and hence applicable to numerous real world problems. The course provides an introduction to conditional and total probabilities along with partitioning of sample space using simulations in Python. You will learn Maximum likehood Estimation (MLE) and Maximum A Priori (MAP) used in Baysian analyses. Using the taught concepts, you will finally implement a supervised classification algorithm called Naive Bayes by using Just Python and Numpy. Learners are expected to have knowledge of Python programming with core libraries and a basic understanding of computational problem solving approaches.

### Objectives
Learners will be able to:
* Derive and explain Bayes theorem and its constituent components (prior, posterior and likelihood). 
* Evaluate the impact of data on posterior probabilities through simulations using python, numpy and matplotlib.
* Implement Naive Bayes algorithm in Python to solve a classification problem and make predictions for unseen data. 
