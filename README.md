# MovieRecomendationSystem

A movie recommendation system, or a movie recommender system, is an ML-based approach to filtering or predicting the users’ film preferences based on their past choices and behavior. It’s an advanced filtration mechanism that predicts the possible movie choices of the concerned user and their preferences towards a domain-specific item, aka movie.

Collaborative Filtering: Collaborative filtering is to discover the similarities on the user’s past behavior and make predictions to the user based on a similar preferecne with other users. This model is then used to predict items (or ratings for items) that the user may have an interest in.

Matrix factorization is a way to generate latent features when multiplying two different kinds of entities. Collaborative filtering is the application of matrix factorization to identify the relationship between items’ and users’ entities. With the input of users’ ratings on the shop items, we would like to predict how the users would rate the items so the users can get the recommendation based on the prediction.

How it works:
*Suppose a user provides ratings for 5 diffrent movies on the scale on 0 to 10, 10 being the highest.
*We take a matrix of 1s and 0s where the rows represent movies and columns represent genres.
*Multiply the column matrix of user ratings with this matrix which gives a list of values of length same ass number of genres.
*This will tell us how much each genre is liked by the user.
*Get the transpose of this and multiply with the oiginal dataframe of movies and sort the values.
*The highest value is the most recommended movie for the user.
