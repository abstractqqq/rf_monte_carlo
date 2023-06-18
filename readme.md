# A Free Exploration.

I started with the following question:

## The Problem:

Given a random forest model, we want to find a good choice for the n_estimator parameter.

We are going to subsample on the feature space for each decision tree in the forest. 

Let's say we have 100 features in total. And we are subsampling 60 features for each decision tree. Ignore depth for now. How many estimators do we need so that we have 99% confidence that each feature is selected at least 3 times? (by different trees)

## Solution with Monte Carlo

I used Monte Carlo simulation to estimate the probablities associated with n_estimators.

## Central Limit Theorem

You will notice that the average count of the times a feature is repeatedly selected follows the random distribution.