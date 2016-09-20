# Building a Better Board Game

For my capstone in the [Udacity Machine Learning Nanodegree program](https://www.udacity.com/course/machine-learning-engineer-nanodegree--nd009), I applied machine learning techniques to a set of data regarding board games. My intent was two-fold:

1. Attempt to fit a model to a set of board game features, in an attempt to predict game ratings.
2. Use this model to provide insight into the characteristics of highly- and poorly-rated games.

The data used in this project come from [BoardGameGeek.com](http://www.boardgamegeek.com/browse/boardgame), and consist of 159 features for each of 84.593 games, each rated by the user community on a 1-10 scale. The ratings were distribued as follows:

![Distribution of Games by Rating](https://raw.githubusercontent.com/rcalme/udacity-capstone/master/img/rating_distribution.png)

I created models using the following learners:
* Random Forest
* K-Nearest Neighbors
* Support Vector Regression
* Gradient Boosting Regression

I stacked the results of the above learners with the LassoCV estimator, and obtained a final model with a correlation of **0.809**.
![Comparative performance of models](https://raw.githubusercontent.com/rcalme/udacity-capstone/master/img/comparative_model_performance.png)

By creating artificial feature vectors, I could approximate 100,000 additional non-existent games, and predict their scores with this model. I then used this data in an attempt to draw some conclusions about highly- and poorly-rated games.

![By category](https://raw.githubusercontent.com/rcalme/udacity-capstone/master/img/by_category.png)
![By mechanic](https://raw.githubusercontent.com/rcalme/udacity-capstone/master/img/by_mechanic.png)

See the [final report](https://raw.githubusercontent.com/rcalme/udacity-capstone/master/Report/Report.pdf) for more detail.
