## [The Model](https://elasticalist.github.io/Model/ "Learn more about the model") | [Model Evaluation](https://elasticalist.github.io/Evaluation/ "Past season performance of the model") | [Upcoming Match Predictions](https://elasticalist.github.io/Upcoming/ "The predictions of the upcoming matches")

# EnglishPremierLeaguePredictor

EnglishPremierLeaguePredictor is a predictor of Premier League games based on historic performances of teams, taking into account their league table statistics. 

## Data Collection and Training

We collected historic data from the league table using [Understat](https://understat.com/ "Understat's Homepage") and its [API](https://understat.readthedocs.io/en/latest/ "Understat API") from 2017 to 2022 for each team, one day before each individual match. This data was then correlated with historic results and odds gathered through [Football-Data.co.uk](https://www.football-data.co.uk/englandm.php "Football-Data.co.uk"). A linear regression algorithm was trained to predict Home Goals and Away Goals.

## Including Form into the Method

To incorporate recent form into our predictions, we repeated the process mentioned above, but only considered the last month of the league table. This allowed us to compute predictions based on the current form of teams. We then implemented a voting system to choose between the season-long prediction and the form-based prediction. Using the Poisson probability density function those predictions were converted to probabilities and the most popular odds of Home Win, Draw, Away Win, Over 2.5 Goals, Under 2.5 Goals and probable scorelines were calculated.


