# Review-Predictor

BoardGameGeek is a very popular site where different types of board games are discussed and reviewed.

In this project, we have a dataset containing 80,000 board games and their corresponding review scores. These data was scraped from BoardGameGeek. The data contains rows and columns, Each row represents a single board game and has statiistics about the board game as well as review information.
Some of the columns are:
Name: The name of the board game
Playingtime: the playing time (given by the manufacturer).
minplaytime: the minimum playing time (given by the manufacturer).
maxplaytime: the maximum playing time (given by the manufacturer).
minage: the minimum recommended age to play.
users_rated: the number of users who rated the game.
average_rating: the average rating given to the game by users. (0-10)
total_weights:Number of weights given by users. Weight is a subjective measure that is made up by BoardGameGeek. It describes how "deep" or involved a game is.
average_weight: the average of all the subjective weights (0-5).

The aim of this project is to predict average_rating using the other columns. Since the dataset contained a few missing values and there were rows without reviews, where there is a score of 0, it was removed.

After using Linear Regression model, I found out that the Mean Squared Error(MSE)=2.078 which is greater than 0, making a Linear model unfit for this prediction, hence we tried the Random Forest Regressor, which was eventually generating prediction value close to the actual values by a tiny fraction.

