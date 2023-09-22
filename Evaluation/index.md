________________________________________________________________________________________________________________________________

## [Home](https://elasticalist.github.io/Home/ "EnglishPremierLeaguePredictor Home page") | [The Model](https://elasticalist.github.io/Model/ "Learn more about the model") | [Model Evaluation](https://elasticalist.github.io/Evaluation/ "Past season performance of the model") | [Upcoming Matches](https://elasticalist.github.io/Upcoming/ "The predictions of the upcoming matches") 

## Model Evaluation
For the hyperparameter optimisation a random shuffling technique was used. The results showed a consistent overperformance of the bookmakers' odds in betting 'Under 2.5 Goals' as depicted below:

![Evaluation of the Under 2.5 Goals betting](ExamplePlotProfit.png?raw=true)
*The performance of Under 2.5 Goals betting on repeated shuffled games. On the upper figure the balance and balance% can be seen with their respective confidence intervals. On the lower figure an indicative betting amount in comparison with the return of the bet can be seen*

As for the other bets the performance was not as consistent, resulting in lower confidence of beating the bookmakers. There are many reasons on why that would be the case ranging from the need of better model tuning to the balancing of the odds of the bookmakers as a result of the betting tendancies of the average bettor. 


Focusing on the 'Under 2.5 Goals' betting we then tested our model using cross-validation, training on all seasons but one and testing it on the hidden season. We test the algorithm on seasons 2017-2022 with consistent positive results. The years 2020-2022 can be seen below:

![Betting on Under in 2020 Season](Under2020.png?raw=true)
![Betting on Under in 2021 Season](Under2021.png?raw=true)
![Betting on Under in 2022 Season](Under2022.png?raw=true)

An example bank of 50 euros is set at the start of the season in order for the model to run as expected. Popular metrics such as [ROI](https://www.investopedia.com/terms/r/returnoninvestment.asp) and and [Net Gain](https://www.investopedia.com/terms/n/netincome.asp) are also shown in the above figures.
