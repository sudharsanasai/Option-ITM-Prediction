# Option-ITM Prediction

We leverage our team’s diverse skill set in combination with an iterative approach and emphasis on bakeoff style testing with minimal to no assumptions to develop a supervised machine learning model to integrate potential predictive features from the realm of technical analysis, volatility modeling, factor exposures, macroeconomic signals, and foreign exchange cross-rates to develop a binary classification algorithm designed to forecast our target variable and place it into one of two categories, Outperform (QQQ must rise at least ten basis points from the start of the 10-day period, from t=0 to t=10) and Underperform otherwise.  Our goal is to develop a supervised learning model that outperforms random prediction with respect to the class expectation for the the 10-day forward returns on the NASDAQ Composite Index (QQQ).  

This paper seeks to evaluate the hypothesis that financial market prices follow a random walk, with little (if any) persistent signal. While cross-checking with an industry practitioner, we emphasize a purely data-driven (assumption-free) approach and iteratively test thousands of model-hyperparameter permutations to test our hypothesis. 

Null Hypothesis 
H0: AUC ~ 0.50  

Alternate Hypothesis
HA: AUC > 0.50 (p-value < 0.05) 

We postulate that any signal that exists in intraday data or over the range of a couple of days degenerates rapidly, crowded out by chaos and complex interconnection of observable features. As such, if our models result in an AUC score that is statistically different from AUC = 0.50 (purely random), we reject the null hypothesis.  
