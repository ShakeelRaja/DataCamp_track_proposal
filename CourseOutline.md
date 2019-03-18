
# Course Outline
## Course 3: Matrix Decomposition Techniques for Machine Learning

## Chapter 1: Understanding Matrix decomposition

This chapter will highlight the need for matrix decomposition with singular matrices that can not be solved through simple linear algebra. You'll be introduced to the general idea of matrix decomposition and some commonly used decomposition techniques for solving systems of linear equations. You will implement LU and Cholesky decomposition methods using NumPy and SciPy libraries in Python. The chapter will compare and contrast matrix decomposition techniques and discuss their suitability for specific application domains.  


* 1.1 Introduction to matrix decomposition
    * Identify matrix decomposition as an important step in solving challenging linear systems in a computationally efficient manner.
    * Compare and contrast different matrix decomposition techniques with their use cases.
    
    
* 1.2 Performing Lower-Upper (LU) matrix decomposition 
    * Apply LU matrix decomposition and reconstruction using SciPy's `scipy.linalg.lu` for solving a system of linear equations.


* 1.3 Performing Cholesky matrix decomposition
    * Create Cholesky matrix decomposition and reconstruction using Numpy's `numpy.linalg.cholesky` method for solving a system of linear equations.

## Chapter 2: The Curse of Dimensionality and PCA

Curse of dimensionality is a topic of huge importance and attracts a lot of attention in the domain of big data analytics. This chapter will introduce you to the problems that analysts have to face while dealing with high dimensional datasets. You will develop a sound geometric understanding of this phenomenon and how it gets worse with the increasing number of dimensions. Although it is hard to visualize data beyond three dimensions, you will run a simple simulation in Python to observe the effect of this problem on sample density and predictive accuracy using a multivariate dataset. The chapter will introduce you to Principle Component Analysis; a common technique used to reduce dimensions of a multivariate dataset while preserving the variance within data elements. 


* 2.1 Introduction to the curse of dimensionality 
    * Describe the curse of dimensionality and the need for dimensionality reduction in high dimensional data, using a geometric explanation with hyperplanes and hypercubes. 
    
    
* 2.2 Understanding multivariate data
    * Describe multivariate data and summarize the role of mean vector and covariance matrix in a multivariate dataset.
    * Create and visualize a multivariate dataset from given mean vector and covariance matrix using Numpy's `numpy.random.multivariate_normal` method. 
    
    
* 2.3 Simulating curse of dimensionality
    * Design and run a simple simulation in Python and Numpy to visualize the effects of high dimensional data on sample space density and accuracy of observed data.


* 2.4 Dimensionality reduction with Principle Component Analysis (PCA)
    * Explain geometrically, how PCA reduces dimensions in high dimensional data while maintaining variance.
    * Define principal components, what do they represent and how many components are needed.

## Chapter 3: Performing Eigendecomposition for PCA

This chapter will take you through the complete PCA process from data pre-processing and preparation, applying PCA to a high dimensional dataset and identifying a lower number of principle components that best describe the data. We will use NumPy in order to simplify the calculation for eigendecomposition and focus more of developing a strong geometric intuition behind the process. You will work with a toy dataset and reduce the number of dimensions from 3 to 2. 

* 3.1 Introduction to eigendecomposition
    * Describe eigendecomposition and the properties of resulting eigenvectors and eigenvalues  
    * Demonstrate eigendecomposition and reconstruction for a given matrix using Numpy's `numpy.linalg.eig` method. 


* 3.2 Pre-processing data for PCA
    * Apply feature normalization to given data prior to PCA.
    * Calculate covariance matrix for the dataset by passing all dimensions of data to Numpy's `numpy.cov`.


* 3.3 Performing eigendecomposition
    * Apply eigendecomposition to calculated covariance matrix using Numpy's `numpy.linalg.eig`. 
    * Sort and Select any given number of EigenVectors that best describe variance in the data.
    * Transform samples to a low-dimensional subspace


* 3.4 Visualizing principle components 
    * Illustrate the effect of PCA on data using 2D/3D scatter plots in MatplotLib.  

## Chapter 4: Singular Value Decomposition for Collaborative Filtering

This chapter will introduce you to a highly sophisticated decomposition technique known as Singular Value Decomposition or SVD. You will see how SVD is a superior approach than eigendecomposition in terms of stability and accuracy of results. You will use SciPy library's built in methods to perform SVD on a subset of MovieLense database for building a collaborative filtering based recommendation system and making recommendations to users for the movies they haven't seen yet. This approach can be easily scaled up to build more sophisticated systems with larger datasets. 


* 4.1 Understanding Collaborative Filtering
    * Describe the role Collaborative Filtering with Utility matrices towards building recommender systems


* 4.2 Singular Value Decomposition (SVD)
    * Recognize SVD as a suprior matrix decomposition technique while comparing it with other approaches. 
    * Explain a solid mathematical intuition behind SVD process. 
    
    
* 4.3 Performing SVD on MovieLense data
    * Create a Utility matrix from subset of MovieLense dataset using Pandas `pandas.pivot`method.
    * Apply SVD to the utility matrix using Scipy's `scipy.sparse.linalg.svds` method. 
    * Convert and reshape sigma factors resulting from SVD using Numpy's `np.diag`. 


* 4.4 Making recommendations
    * Calculate predictions from decomposed matrices for movie ratings predictions for every user.
    * Create a function `recommender()` for recommending top new movies based on the predictions. 
