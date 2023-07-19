# ML-Homework

A more detaild description of the dataset can befound here https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset

## Roadmap

### 1. Preliminary analysis
#### 1.1 Data inspection
* visualize samples
* identify if features are correlated
* determine which are the most correlated with the target class
* inspect the distribution of samples among classes
#### 1.2 Exit Rate regression
* train a regressor to predict the values of this variable, given the remaining ones
* compare different regression algorithms for this task -> use robust evaluation techniques to compare the algorithms
* perform feature selection
This feature is also missing in the test set, so we have to use only the training data for this step

### 2. Classification
* use the regression model trained at the previous step to recover exit rate by predicting their value for each missing sample on the train and test set.
* build a classification model to correctly predict if an online shopper is likely to perform a purchase.
* perform feature selection
* compare different algorithms and identify the one that works the best on this dataset
* test the performance of the best algorithm on the provided dataset
* determine whether a model built using the exit rate information is better than a model bult using the remaining features

### 3. Clustering
* Repeat the analysis done at step 3 with clustering algorithms
* compare their performances wrt a classification model
