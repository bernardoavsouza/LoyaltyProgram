# Loyalty Program

This repository contains code and documentation for a data science project. The main goal of this project is to create a loyalty program for e-commerce. All the data used was provided by Kaggle.


# 1. Business Problem

A well-designed loyalty system is essential in building long-term customer relationships, driving repeat business, and enhancing brand loyalty. It enables businesses to reward customers, encouraging repeat purchases and promoting customer engagement. Incorporating machine learning into this system can greatly enhance its effectiveness by enabling personalized offers and rewards, based on individual customer behavior and preferences. This level of personalization and predictiveness can significantly increase customer satisfaction, loyalty, and ultimately, business revenue.


# 2. Business Assumptions

The main assumption considered in this project was the main goal of raising the gross revenue.


# 3. Solution Strategy

### Step 1: Data Description

The main objective of this section was to organize and understand raw data using descriptive statistics.

### Step 2: Variable Filtering

This step was responsible for dropping records that were not about purchases.

### Step 3: Feature Engineering

In this step, a DataFrame of Features was created. Time-based features were built considering the last 90 days.

### Step 4: Exploratory Data Analysis

This step consisted of three different analyses: univariate, bivariate, and embedding space analyses. The univariate analysis was conceived in Pandas Profiling and the embedded spaces considered for the analysis were PCA, t-SNE, and UMAP.

### Step 5: Feature Selection

In this section, the previous analyses were used to select the best features to be used in the algorithm.

### Step 6: Data Preparation

In this section, the data were scaled to perform properly in a machine learning algorithm. Moreover, the data were subject to a tree-based embedding.

### Step 7: Hyperparameter Fine Tunning

The data were analyzed with the elbow method and the silhouette method. After that, three different clustering algorithms were tested: K-Means, Hierarchical Clustering, and Gaussian Mixture Model.

### Step 8: Machine Learning Modelling

Here, the best choice of algorithm and the number of clusters were evaluated as the final model.

### Step 9: Cluster Analysis

This step was responsible for visualizing graphically the final result of the obtained clusters. Moreover, the profile of each cluster was analyzed as well.

### Step 10: Exploratory Data Analysis II

The main objective of this section is to answer some business questions.


# 4. Top 3 Data Insights

**Hypothesis 1: _Premium_ customers bring more than 50% of the total revenue.**

**True:** Premium customers bring 53.16% of the total revenue.

**Hypothesis 6: Cluster _Gold_ I, _Sub Premium_, and _Premium_ customers added up bring more than 80% of the revenue.**

**False:** They bring around 71.38%.

**Hypothesis 2: More than 50% of the items sold are bought by _Premium_ customers**

**True:** Around 56.46% of the items sold were bought by _Premium_ customers


# 5. Machine Learning Model Applied

In this project, three machine learning models were tested: K-Means, Hierarchical Clustering, and Gaussian Mixture Model. The final model was built using K-Means with K = 11.


# 6. Machine Learning Model Performance

The final model was built with a silhouette score of 62.2% and a Within-Cluster-Sum of Squared Errors of 30920.22.


# 7. Business Results

The algorithm was capable of creating a customer segmentation that clustered 11 groups of customers. Therefore, it was possible to raise a table with details about all 11 kinds of customers and create a hierarchy based on their influence on gross revenue.


# 8. Conclusions

Therefore, a machine learning algorithm can be used to segment customers based on how they impact gross revenue, enabling the company to make informed decisions about creating a loyalty system. Thereby, operation planning such as marketing campaigns came to be accurate and unbiased with this method. 


# 9. Next Steps to Improve

The next improvement to be sought will be to test other algorithms, such as Mean Shift or DBSCAN. Moreover, it is possible to develop a classification algorithm that classifies in which cluster a new customer will be allocated.
