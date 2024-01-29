# Sampling-Dhruv-102117061
# Sampling Techniques and Model Accuracy Analysis

## Overview

This document presents an analysis of different sampling techniques applied to a dataset with an initial imbalance (763 non-fraudulent cases and only 9 fraudulent cases). To address this, an oversampling approach was used to balance the dataset. Five distinct sampling techniques were employed to generate representative samples, followed by the application of various models to each sample.

## Sampling Techniques Used

1. **Simple Random Sampling**: Samples are randomly selected from the population.
2. **Systematic Sampling**: Samples are selected at regular intervals after a random start.
3. **Cluster Sampling**: Entire clusters are randomly selected from the population.
4. **Stratified Sampling**: The population is divided into subgroups (strata), and samples are taken from each stratum.
5. **Bootstrap Sampling**: Samples are created by resampling with replacement from the original dataset.

## Models Applied

The following models were applied to each sample:

- Random Forest
- Logistic Regression
- SVM (Support Vector Machine)
- Decision Trees
- Gradient Boosting

## Model Accuracy Results

The accuracies of each model for the respective sampling technique are summarized in the table below:

| Sample Technique        | Random Forest | Logistic Regression | SVM    | Decision Trees | Gradient Boosting |
|-------------------------|---------------|---------------------|--------|----------------|-------------------|
| Simple Random Sampling  | 1.0000        | 0.8993              | 0.9530 | 0.9930         | 1.0000            |
| Systematic Sampling     | 1.0000        | 0.8926              | 0.9530 | 1.0000         | 1.0000            |
| Cluster Sampling        | 1.0000        | 0.8926              | 0.9530 | 1.0000         | 1.0000            |
| Stratified Sampling     | 1.0000        | 0.8926              | 0.9530 | 1.0000         | 1.0000            |
| Bootstrap Sampling      | 1.0000        | 0.8926              | 0.9530 | 1.0000         | 1.0000            |

## Conclusion

In this analysis, the **Random Forest**, **Decision Tree**, and **Gradient Boosting** models all achieved 100% accuracy across all sampling techniques, showcasing their effectiveness in handling the balanced dataset.

