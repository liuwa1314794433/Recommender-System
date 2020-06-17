# Item-based Collaborative Fitering


##Item based nearest neighbor CF

 Step 1: Calculate Similarity between an item and all the rest of the items.  

 Step 2: order items by similarity.Use an ordering algorithm, the choice is not impacting on the algorithm.  

 Step 3: Select the neighbourhood.  

 Step 4: Compute the predicted rating for the item.  


## Model based approach
- Offline pre processing or "model learning" phase.
- At run time, make predictions only using the learned model.
- Models are updated/re trained periodically.
- Large variety of techniques.
- Computationally expensive model building and updating.
- Item based CF is an example for model based approaches.
