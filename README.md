# Model-Evaluation

## Recommender Systems

Bootstrap is a statistical resampling technique that is used to estimate the quality of a model. It involves creating a large number of random samples with replacement from a dataset and using each of these samples to build and evaluate a model. By aggregating the results from each of these models, we can get a more accurate estimate of the model's performance.

In this exercise, we will use bootstrapping to estimate the generalization error of the K-nearest neighbors (KNN) algorithm using various metrics including f1 score, accuracy, recall, and precision. Follow the instructions below and report the results:

For each metric, repeat the following process 100 times:

* Randomly select 10% of the data as the test set.
* Split the remaining 90% of the data into a training set and a validation set (in a 90/10 ratio).
* Fit the KNN model for different values of K and evaluate the validation performance according to the selected metric.
* Determine the best value of K based on the validation performance.
* Estimate the performance of the KNN model with the best K using the test set.

Finally, for each metric, calculate the average performance across the 100 executions for each metric.
