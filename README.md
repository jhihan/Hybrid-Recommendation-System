# Hybrid-Recommendation-System
Build up a hybrid recommender system based on MovieLens database using content-based filtering and collaborative filtering algorithms
## Movie Recommendation System Development
A recommender system, or a recommendation system is a subclass of information filtering system that seeks to predict the "rating" or "preference" a user would give to an item. Recommendation systems can produce produce the prediction in Content-based filtering or Collaborative filtering. In this project, a hybrid approach is used to build up a recommendation system in the Colab notebook.
### Setup
```Shell
pip install fuzzywuzzy
pip install surprise
```
### Datasets
The datasets used in this project are from [MovieLens Datasets](https://grouplens.org/datasets/movielens/latest/). There are smaller datasets which contain 100,000 ratings and 3,600 tag applications applied to 9,000 movies by 600 users. There are also full datasets which contains 27,000,000 ratings and 1,100,000 tag applications applied to 58,000 movies by 280,000 users. Here the smaller datasets are used as the practice.
### Models
This recommendation system is built up with the Hybrid model using content-based filtering and collaborative filtering:
* Content-based filtering: the cosine similarity between vectors in tf-idf Vector-Space model is used
* Collaborative filtering:
   Singular Value Decomposition (SVD) matrix factorization algorithm from the Surprise package is used.
   Alternating Least Square (ALS) matrix factorization algorithm in the PySpark framwork is used. (in Recommendation_system_pyspark.ipynb)
### Recommendation
With a given user Id and a favorate movie name, the two recommendation lists from the content-based filtering and collaborative filtering are shown. The result from the content-based filtering recommends us the movies which are similar to the input favorate movie according to the genres in the datasets. The result from the collaborative filtering recommends us the movies which other users who are similar to us also like.
## Outlook
* Impliment the recommendation system in Pyspark framewrke in order to perform large-scale data processing and machine learning algorithms.
* Productionize existing code.
## References
https://en.wikipedia.org/wiki/Recommender_system
