# Hybrid-Recommendation-System
Build up a hybrid recommender system based on MovieLens database using content-based filtering and collaborative filtering algorithms
## Movie Recommendation System Development
### Datasets
The datasets used in this project are from [MovieLens Datasets](https://grouplens.org/datasets/movielens/latest/). There are smaller datasets which contain 100,000 ratings and 3,600 tag applications applied to 9,000 movies by 600 users. There are also full datasets which contains 27,000,000 ratings and 1,100,000 tag applications applied to 58,000 movies by 280,000 users. Here the smaller datasets are used as the practice.
### Models
This recommendation system is built up with the Hybrid model using collaborative filtering and content-based filtering:
* Collaborative filtering:
   Singular Value Decomposition (SVD) matrix factorization algorithm from the Surprise package is used.
* Content-based filtering: the cosine similarity between vectors in tf-idf Vector-Space model is used
