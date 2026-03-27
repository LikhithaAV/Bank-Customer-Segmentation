# Bank-Customer-Segmentation

This repository contains a machine learning project focused on bank customer segmentation based on their credit card usage and interaction patterns.

## Notebook Overview

The Clustering.ipynb notebook utilizes unsupervised Learning techniques, specifically K-Means Clustering and Hierarchical Clustering, to identify distinct customer groups. By understanding these segments, banks can tailor their marketing strategies, improve customer service, and optimize credit offerings.

## Problem Statement

Modern banks handle vast amounts of customer data but often struggle to provide personalized experiences. The goal of this analysis is to:
1. Identify different segments of credit card customers based on their financial behavior and communication preferences.
2. Provide actionable insights into each segment to help the bank's marketing team target the right customers with appropriate products (e.g., credit limit increases)

## Dataset Source

The data is sourced from GitHub.

## Key Concepts 

| Feature                  | Description                                         |
|--------------------------|-----------------------------------------------------|
| Avg_Credit_Limit         | Average credit limit assigned to the customer |
| Total_Credit_Cards       | Total number of credit cards held |
| Total_calls_made         | Number of calls made to customer support |
| Total_visits_bank        | Frequency of physical bank visits |
| Total_visits_online      | Frequency of online banking logins |

## Notebook Structure

The analysis is organized into the following logical sections:
1. Imports and Data Loading: Setting up the environment and loading the CSV file.
2. Data Cleaning: Checking for missing values and removing duplicate entries to ensure data integrity.
3. Exploratory Data Analysis (EDA): Visualizing the data through various plotting functions (labeled_barplot, histogram_boxplot) to gain initial insights.
4. Outliers Detection and Removal : Uses a custom histogram_boxplot function to visualize the distribution and identify extreme values across features like Avg_Credit_Limit and Total_visits_online.
5. Data scaling : aPPLY StandardScaler to standardize the features.
6. Model Training and Evaluation: Uses K-means and Hierarchical Clustering to create clusters and verify with Silhouette score
   * K-Means Clustering: Implementing the K-Means algorithm and evaluating results via the Elbow method.
   * Hierarchical Clustering: Performing agglomerative clustering and analyzing the resulting dendrogram.
