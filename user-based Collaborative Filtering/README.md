# User-based Collaborative Filtering


## User based nearest neighbor CF

  Data requirements for successful CF.Data should be well connected.If no user rated content you cannot make  
recommendations.Users without overlapping tastes with other users won't receive good recommendations.

## CF algorithms don’t require any domain knowledge.

Step 1: Calculate Similarity between the active user and the rest of the users.A popular similarity measure in user based CF:   
        Pearson correlation coefficient.Compute the similarity for each user.Reduce the number of comparisons.  

Step 2: order user by similarity.Use an ordering algorithm, the choice is not impacting on the algorithm.  

Step 3: Select the neighborhood.Neighbors selection can be made using like Clustering,Top k,Threshold on similarity.Clustering is mostly         used for Item based CF.Selecting threshold and k can be challenging,depending on how well the similarity measure differentiates         the between the users.  

Step 4: Compute the predicted rating for the item.Only the ones that all the other neighboring users have  
        rated.Give a value of number of co rated items.Not all neighbor ratings might be equally "valuable".  


## User based CF is said to be "memory based"
- Directly use the rating matrix to find neighbors and make predictions.
- Does not scale for most real world scenarios.
- Large e commerce sites have tens of millions of customers and millions of items.

## Model based approaches
- Offline pre processing or "model learning" phase.
- At run time, make predictions only using the learned model.
- Models are updated/re trained periodically.
- Large variety of techniques.
- Computationally expensive model building and updating.
- Item based CF is an example for model based approaches.
