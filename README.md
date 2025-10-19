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

First improtant thing to do is understand the data , we will do EDA (Book : Practical Statistics for Data Scientist) and Kaggle excerise will be used for this purpose. 

# Chapter 01 : Exploratory Data Analysis  
Data comes from many sources: sensor measurements, events, text, images, and videos. The Internet of Things (IoT) is spewing out streams of information. Much of this data is unstructured: images are a collection of pixels, with each pixel containing RGB
(red, green, blue) color information. Texts are sequences of words and nonword characters, often organized by sections, subsections, and so on. Clickstreams are sequences of actions by a user interacting with an app or a web page.
Datatypes:
    Numeric:        
        Continuous and Discrete
    Categorical:
        Data can take specific set of values representing that category.
        Binary : 0 and 1
        Ordinal : explilicit ordering (like rating a restraunt )
Data typing in software acts as a signal to the software on how to process the data
When we have data ,we need to find something which can represent the whole data I mean **Central tendency**.
Few methods of these estimation are :
    * Mean: average (sensitive to outliers)
    * Weighted mean : give more important to some data points over others.
    * Median : half data like above half below (50 percentile)
    * Trimmed mean : The average of all values after dropping a fixed number of extreme values (Truncated mean).
    * Percentile : The value such that P percent of the data lies below.
But **Central tendency** can not represnt the whole data so study of **Variablity or spread** is also important .
Some of key terms to study variablity are:
    * Deviation : The difference between the observed values and the estimate of location. (error or residue)
    * Variance : The sum of squared deviations from the mean divided by n – 1 where n is the number of data values.
    * Standard deviation : Root of Variance (same unit as measurement)
    * Mean absolute deviation : The mean of the absolute values of the deviations from the mean (second norm).
    * Median absolute deviation from the median : The median of the absolute values of the deviations from the median.
    * Range : The difference between the largest and the smallest value in a data set. (outlier sensitive)
    * Order statistic : Metrics based on the data values sorted from smallest to biggest (rank).
    * Percentile : The value such that P percent of the values take on this value or less and (100–P) percent take on this value or more.
    * Interquartile range : The difference between the 75th percentile and the 25th percentile. (IQR)

One of the subtle difference that I noticed was **Quantile**,**percentile**,**Quarntile**
**Quantile**: A value that divides a probability distribution or a dataset into equal-sized, continuous intervals. (0 to 1)
**Percentile**: A specific qunatile that divides dataset into 100 equal parts.
**Qarntile**:  A specific qunatile that divides dataset into 4 equal parts.

Calculating percentile is very computationlly heavy specifically for large data set.