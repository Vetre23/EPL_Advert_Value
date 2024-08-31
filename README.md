Premier League Advertisement Value Prediction


Project Overview


This project aims to predict which Premier League teams offer the highest advertising potential based on a combination of player performance, match results, and engagement metrics such as Instagram followers and top player interaction points.


Data Sources


The datasets used in this project include:

Player Performance Data: 

Metrics such as goals scored, assists, clean sheets, and more.
Match Events Data: 

Information about each match including goals, xG (expected goals), and xGA (expected goals against).
Engagement Metrics: 

Instagram followers, player interaction points, and other fan engagement data.


Data Preparation

Data Cleaning

Missing values were identified and handled appropriately.

The datasets were merged using relevant keys such as teamId.


Feature Engineering

New features were created to represent player and team performance, including composite scores for player value and engagement.
Teams' performance was analyzed using xG, xGA, and actual goals scored or conceded.


Modeling Approach

Target Variable Creation


The target variable (advertisement_value) was created using thresholds based on quantiles of key performance metrics such as wins, goals scored, and Instagram followers.


Logistic Regression


A logistic regression model was used to predict the binary target variable.

Hyperparameter tuning was performed using GridSearchCV to optimize the model.


Results


Feature Importance: Key features influencing advertisement value were identified.


Top Teams: The model highlighted teams with the highest predicted probability of high engagement, which could be potential candidates for advertisement investment.


Conclusion


The analysis identified critical factors that contribute to a team's advertising value, emphasizing the importance of player performance and fan engagement metrics. The model's predictions can guide decision-makers in selecting the best teams for advertisement investments.


Future Work


Incorporate More Data:

Adding more engagement metrics such as viewership data could improve the model's accuracy.

Advanced Modeling Techniques: 

Experimenting with other models like Random Forest or Gradient Boosting could provide better predictive performance.
