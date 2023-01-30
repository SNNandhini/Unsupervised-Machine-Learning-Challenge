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

![image](https://user-images.githubusercontent.com/111614210/215368519-6d5f3c08-1e31-4915-abfd-4d17e8eefb03.png)

## 2)   Apply Dimensionality Reduction
-   Perform dimensionality reduction with PCA, preserving 90% of the explained variance in dimensionality reduction.

![image](https://user-images.githubusercontent.com/111614210/215368832-38a8d80c-7926-4d55-bb61-80f3bdbcab9c.png)
![image](https://user-images.githubusercontent.com/111614210/215368897-6736a111-2951-4712-8190-0228f33b08bb.png)

-   Further reduce the dataset dimensions with t-SNE and visually inspect the results. To do this, run t-SNE on the principal components, which is the output of the PCA transformation.

![image](https://user-images.githubusercontent.com/111614210/215369019-c01208c9-2837-4d47-a665-6080f366f35d.png)

-   Create a scatter plot of the t-SNE output.

![image](https://user-images.githubusercontent.com/111614210/215369592-af1b211e-771b-4677-8567-3aa1301ffaee.png)

Scatter Plot coloured by target value (MYOPIC column from the original dataset)

![image](https://user-images.githubusercontent.com/111614210/215369266-1754c5bc-56ff-4145-b7a4-c06ef42946b6.png)

## 3)   Perform a Cluster Analysis with K-means
-   Create an elbow plot to identify the best number of clusters.

![image](https://user-images.githubusercontent.com/111614210/215369365-a0358de0-1949-4a39-9e50-824a68809190.png)

## 4)   Make a Recommendation  
-   Based on the findings, write up a brief (one or two sentences) recommendation.

![image](https://user-images.githubusercontent.com/111614210/215369456-4321717a-f8c1-4c6a-86e1-2469065fb202.png)

## Files Uploaded
-   **Jupyter Notebook**: Myopia_Cluster_Analysis.ipynb
-   **Input File**: Resources/myopia.csv
