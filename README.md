# Movie-Rating-Prediction-from-IMDB-Dataset
1- We used a dataset that only includes movies after the year 2000. We narrowed down the movies that had at least 10,000 raters and a budget of at least 10,000 USD.

This was done in order to eliminate the newer movies which did not have enough ratings submitted to be fairly judged and would reduce the accuracy of the data.

2- There were also an amount of very low budget movies which traditional movies in the sense so we set the budgetary limit to eliminate those movies from causing errors in our predictions as well.

3- For the “Rated” column in our dataset, we used a onehot encoder to convert the category names of the column into values in order to ease prediction calculations. We also
used one-hot encoder for the “Genre” column to convert them to zeros and ones, the “Directors” column but narrowed the selection down to only the top 10 directors, the “Actors”
column but narrowed it down to the top 20 actors and lastly the “Production Company” but only to the top 10 companies.

4- We added an extra column to the dataset that calculates the time in years difference between now and the time of movie releasing. 

5- We classified the data by converting the IMDb ratings into three categories: category 0, category 1, category 2. The target labels were 0-4 for category 0, 4-7 for category 1, and 7-10 for category 2. 

6- There were two steps for our data classification: Data testing and Data training. We used 75% of the data as training data and the remaining 25% was used for training. We utilized multiple data classifiers to do perform these data classifications in order to maximize prediction accuracy by choosing the classifier that yields the most accurate results. We compare between GradientBoosting, Random Forest, KNN, and Extratrees classifiers to classify the dataset.
