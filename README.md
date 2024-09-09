# movie-recommender
This project implements a movie recommendation system using collaborative filtering. The system predicts how a user would rate a movie they haven't seen yet by finding movies similar to those they've already rated and considering the ratings of other users. The dataset is derived from the MovieLens 100k dataset, which contains user ratings for different movies.

Explanation of Key Steps:
Data Loading and Merging: This step merges user ratings with movie titles, so each user's rating is associated with the correct movie.
User-Movie Matrix: A user-movie matrix is created to facilitate comparisons between users and movies.
Correlation Matrix: The Pearson correlation between movies is calculated to determine how similarly users rate different movies.
Scaling and Penalizing: Ratings are scaled based on the user's preferences, and movies similar to those disliked by the user are penalized to improve recommendation quality.
Prediction: Ratings for unseen movies are predicted by finding how similar movies were rated by the user.
