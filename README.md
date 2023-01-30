# Unsupervised-Machine-Learning-Challenge
Myopia Clusters

This Challenge is to apply unsupervised learning by fitting data to a model and using clustering algorithms to place data into groups.

The data used for this challenge is from a medical research company that’s interested in finding better ways to predict myopia, or nearsightedness. The goal is to find out whether the patients can be placed into distinct groups for effective analysis. 

The steps followed for this challenge are as follows:
## 1)   Prepare the Data
-   Read the input file (Resources/myopia.csv) into a Pandas DataFrame.
-   Remove the target column (MYOPIC) from the dataset, as it will make an unsupervised model biased.
-   Standardize the dataset so that columns that contain larger values do not influence the outcome more than columns with smaller values.

The data after all preprocessing is as follows:

## 2)   Apply Dimensionality Reduction
-   Perform dimensionality reduction with PCA, preserving 90% of the explained variance in dimensionality reduction.
-   Further reduce the dataset dimensions with t-SNE and visually inspect the results. To do this, run t-SNE on the principal components, which is the output of the PCA transformation.
-   Create a scatter plot of the t-SNE output.

## 3)   Perform a Cluster Analysis with K-means
-   Create an elbow plot to identify the best number of clusters.

## 4)   Make a Recommendation  
-   Based on the findings, write up a brief (one or two sentences) recommendation.

## Files Uploaded
-   **Jupyter Notebook**: Myopia_Cluster_Analysis.ipynb
-   **Input File**: Resources/myopia.csv