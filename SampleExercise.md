
# Sample Exercise
(From section 3.3 in the Course outline)

**Note:** *Sample exercise is slightly longer than outlined in the task brief. The exercise contains 5 bulleted instructions (instead of 4), covering 3 learning objectives (instead of 1 or 2) from section 3.3 in the course outline. This was decided to allow practicing the standard 5-step PCA process as highlighted in PCA literature using a single exercise. If required, this exercise can be borken down into two separate exercises.*

### Introduction: 
Previously, we applied the preprocessing and data preparation routines for getting our 3 dimensional toy dataset (`samples`) ready for PCA. After Calculating the mean vector `mean_vector` and covariance matrix `cov_matrix` in the previous exercise, we are now ready for perform PCA for reducing the number of dimensions in our dataset from 3 to 2. This involves a series of 5 steps as listed below: 

1. Perform eigendecomposition of the covariance matrix using `np.linalg.eig` to calculate eigen components i.e. `eigen_value` and `eigen_vector`. 

2. Make an aboslute list `eigen` of (eigenvalue, eigenvector) tuples by combining each `eigen_value` to corresponding `eigen_vector` iteratively using list comprehension.  

3. Use a lambda function to sort the the `eigen` list ranking from high to low using `reverse=True` argument.

4. Create the dxk matrix from eigenvectors having top 2 eigenvalues (d= number of original dimensions, k = number of principle components). Use `np.reshape()` to reshape top 2 eigenvectors and stack them horizontally using `np.hstack` to create a `dk_matrix`. 

5. Take a dot product of `dk_matrix` with original data `samples` to transform the data into new subspace `transformed` and view the output. 

## Exercise: Performing eigendecomposition for PCA 

```python
# 1. Eigendecomposition - returning eigenvectors and eigenvalues
eigen_value, eigen_vector = _____(_____)

# 2. Make a list of (eigenvalue, eigenvector) tuples
eigen = [(np.abs(_____[i]), _____[:,i]) for i in range(len(_____))]

# 3. Sort the tuples from high to low
_____.sort(key=lambda x: x[0], _____)
print(eigen)

# 4. Create a new dxk matrix by transforming the 3-dimensional feature space to a 2-dimensional feature subspace
dk_matrix = np._____((_____.reshape(3,1), _____.reshape(3,1)))

# 5. Bring original data into the transformed subspace
transformed = dk_matrix.T.dot(samples)
```

## Solution

```python
# 1. Eigendecomposition - returning eigenvectors and eigenvalues
eigen_value, eigen_vector = np.linalg.eig(cov_matrix)

# 2. Make a list of (eigenvalue, eigenvector) tuples
eigen = [(np.abs(eigen_value[i]), eigen_vector[:,i]) for i in range(len(eigen_value))]

# 3. Sort the tuples from high to low
eigen.sort(key=lambda x: x[0], reverse=True)

# 4. Create a new dxk matrix by transforming the 3-dimensional feature space to a 2-dimensional feature subspace
dk_matrix = np.hstack((eigen[0][1].reshape(3,1), eigen[1][1].reshape(3,1)))

# 5. Bring original data into the transformed subspace
transformed = dk_matrix.T.dot(samples)
```

```python
# Let's examine our final output
print (transformed)
```

### Expected Output 
```python
[[ 0.10911892  1.1127986   1.47520878  0.2452085  -0.39569667 -1.13397776
  -0.42276516  1.177862    1.35221667 -2.41786731  2.76142467  1.27089707
   0.66684294 -1.19400131 -0.32399714 -0.40993035 -1.72488793 -0.46104713
  -0.4319508  -0.69772913 -0.89968745 -0.65040799 -1.9739113  -1.96183462
  -2.30947115 -1.01893577 -2.30176836 -1.42346091 -3.11384268 -2.00710413
  -1.48148629 -0.3824814  -1.16617082 -0.44681843 -1.72170484 -2.98473249
  -3.7823004  -3.70587856 -1.32584127 -3.81066259]
 [ 0.11652046 -0.98634218  0.3755543   0.55628868 -0.83469572  0.80649013
  -0.50629116 -0.21266525 -1.28489809  0.19484413 -0.06568692  0.74798017
  -0.64597596 -2.02415723 -1.05608974 -1.18084883  1.85965185 -0.99696254
   0.05931891  0.31474419 -0.39231823 -0.57832542  1.11964987 -3.43207312
  -0.68688666  1.50410004  0.44931099  0.21132585  0.09835353  1.55140177
   1.62374754  1.45949476  1.24065851 -0.1208321  -0.40257785  0.19542387
  -1.22365666 -0.40315698  0.18386443 -0.94137547]]
```

## Feedback 

GREAT, we have now successfully transformed our data from a 3 dimensional feature space to a 2 dimensional subspace as shown in the output array. However, in order to fully appreciate the effect of PCA, we will next visualize the data before and after PCA using 3D and 2D scatter plots to visually inspect how PCA reduces dimensions while preserving variance between observations.
