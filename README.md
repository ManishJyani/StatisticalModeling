# StatisticalModeling
To build statistical model and Get inference from the data
First thing first :
---What is difference between statistical modeling and ML modeling ?  
    Statistical Modeling: Primary goal = Understanding relationships (inference)  
    Machine Learning: Primary goal = Accurate predictions (prediction)  
The confusion arieses due method like Linear regression ,which is labelled as statistical method and ML method some time .  

Same algorithm, different purposes:

Statistics: Interpret coefficients, test hypotheses

ML: Optimize prediction accuracy on test data

It "becomes ML" when you focus on train/test splits, cross-validation, and generalization performance

Some of the comman confusons and there answers:

  Q. How is linear regression both statistics and ML?

  A. Statistics: Uses it for understanding relationships

     ML: Uses it for making predictions

  Q. If I have coefficients, can't I just predict?

  A. Yes, but ML focuses on optimizing those predictions and testing generalization

  Q. Do we never use statistical models for prediction?

  A. Correct - prediction is a byproduct in statistics, but the primary goal in ML

  Q. What about polynomial/logarithmic functions?"

  A. Statistics: Choose form based on theory

     ML: Try multiple forms, pick what predicts best


# Different type of Statistical approachs: 

1. Generalized Linear Models (GLMs)  
    * Logistic Regression: Binary outcomes (yes/no)  
    * Poisson Regression: Count data  
    * Multinomial Regression: Multiple categories  

2. Analysis of Variance (ANOVA)  
    * Compare means across multiple groups  
    * One-way ANOVA: Single factor  
    * Two-way ANOVA: Multiple factors with interactions  

3. Time Series Analysis  
    * ARIMA: Auto-regressive integrated moving average  
    * Seasonal Decomposition: Trend + Seasonality + Residuals  
    * Stationarity Testing: Dickey-Fuller test  

4. Survival Analysis  
    * Kaplan-Meier: Survival curves  
    * Cox Proportional Hazards: Factor effects on survival time  

5. Multivariate Methods  
    * Principal Component Analysis (PCA): Dimension reduction  
    * Factor Analysis: Latent variable discovery  
    * Cluster Analysis: Group similar observations  
 
6. Bayesian Methods  
    * Bayesian Inference: Probability-based parameter estimation  
    * Markov Chain Monte Carlo (MCMC): Complex posterior sampling  

7. Non-Parametric Tests  
    * Mann-Whitney U: Non-normal group comparisons  
    * Kruskal-Wallis: Multiple group comparisons  
    * Spearman's Rank: Non-linear correlations  

8. Experimental Design    
    * A/B Testing: Treatment vs control  
    * Randomized Controlled Trials: Gold standard for causality  
