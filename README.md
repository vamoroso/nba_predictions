# nba_predictions
Code that uses Spark to explore and predict shots made using NBA data.  All of these steps were performed using Pyspark.  Even though the size of the data is manageable in one single computer, I display how a Spark context can be leveraged for faster hyper-parameter tuning in a machine learning problem. Took advantage of spark SQL for more efficient data exploration and filtering.

### Goal
* The goal of this project was to predict whether a shot will be made or missed by an NBA Player. 

### Data
* The data was hosted on Kaggle and pulled from the NBA Rest API.  

### Features
* The features included were shot number, dribbles, touch time, shot distance, point type, defender distance, shot clock, dribbles per second and whether the defender was a matching position to the shooter in question.

### Results
* Obtained an accuracy of 62% and discovered what the best features are for determining an accurate shot or not.  Creating new interaction features such as shot distance * distance to closest defender gave me insight into other interesting relationships between predictors. For example, going in I had a hypothesis that distance from the basket alone would be the best predictor, but as it turned out, the shot distance along with defender distance proved to be a better indicator of whether the shot would be made. 
