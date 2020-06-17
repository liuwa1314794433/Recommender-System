# Matrix Factorization and SVD

## Making recommendations
- Two ways you can make recommendations directly.  
- Compute all predicted ratings, take the largest ones that the user hasnt seen before.  
- Iterate through each item and find similar products in the reduced space.  


## A third, indirect, way is to use the new matrices to compute neighborhood collaborative filtering.  
- Might solve the sparsity problem of those algorithms.  
- These matrices are dense.  
- Higher chances of finding similar items or users.  


## SVD recap
- Optimal decomposition parameter can be determined and fine tuned using also optimization techniques.  
- Stochastic Gradient Descent using Frobenius Norm evaluation.  

## We can add features to the rating computation for additional precision 
   Biases specific for the domain.
    - Combine implicit and explicitfeedback.
    - emporal dynamics.

### Pro
- Easy to insert new users as they arrive.
- Can use implicit and/or explicit feedback.

### Cons
- No unfilled cells in the ratings matrix, should take action before computing.
- Slow to compute large matrices.
- Model is static, should be updated frequently.
- SVD isn’t at all explainable.

# Funk SVD is an improved SVD approach

## Use a machine learning approach to find the best decomposition.
- Doesn’t make use of the Σmatrix.
- Compute the Root Mean Square Error (RMSE) between the predicted and known ratings.
- Optimise the RMSE using stochastic gradient descent.


### Pro
- No need to fill the ratings.
- Works with sparse ratings.

### Cons
- Difficult to add users and items.
- Need time to train.
