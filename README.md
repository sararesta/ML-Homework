# ML-Homework 2022/2023
 * Authors: Valentina Margiotta, Sara Resta
 * Course: Machine learning
 * A.A.: 2022/2023
 * Professors: Matteo Matteucci, Stefano Samele
 * Grade: 6/6
  
-------------------------------------------------------------
    
# Project guidelines
In this project, we aim to use the Online Shoppers Purchasing Intention dataset to
build a classification model that can predict whether or not an online shopper has
the intention to make a purchase.  
  
## Background
The Online Shoppers Purchasing Intention dataset is a publicly available dataset
that contains information on the browsing behavior and purchase history of online
shoppers. The dataset contains different sessions, and it was formed so that each
session would belong to a different user in a 1-year period to avoid any tendency to
a specific campaign, special day, user profile, or period. The dataset has been made
available on the UCI Machine Learning Repository.
  
## Dataset Composition
The dataset contains just over 12,000 samples and includes both categorical and
continuous variables. The categorical variables include information on the type of
the operating system, the region of the shopper, and whether or not the shopper was
a returning visitor. The continuous variables include information on the duration of
the visit, the number of pages visited, and the exit rate, among others.
We have provided you with a particular version of this dataset. There are two files
representing the training set and the test set. For the purposes of this project, we
have corrupted a significant amount of samples of the Exit Rate variable.
  
## Project Steps and requests
 1. Perform preliminary analysis of the data. For instance, but not limited to
    visualizing samples, identifying if features are correlated, determining which
    are most correlated with the target class, and inspecting the distribution of
    samples among classes. We want to recover from the data loss of the Exit
    Rate variable. Train a regressor to predict the values of this variable, given
    the remaining ones. Compare different regression algorithms for this task,
    and perform features selection. Since this feature is also missing in the test
    set, use only the training data for this step and use robust evaluation
    techniques to compare algorithms.
 2. Use the regression model trained at the previous step to recover Exit Rate by
    predicting their value for each missing sample on the train and test set. Build
    a classification model to correctly predict if an online shopper is likely to
    perform a purchase. Perform features selection, compare different algorithms,
    and identify the one that works the best on this dataset. Finally, test the
    performance of the best algorithm on the provided test set. Determine
    whether a model built using the Exit Rate information is better than a model
    built using the remaining features.
 3. Repeat the analysis done at step 2 with clustering based algorithms; compare
    the performance with respect to the best classification model.
  
A more detaild description of the dataset can befound here https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset
