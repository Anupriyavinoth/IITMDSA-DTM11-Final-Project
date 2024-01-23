## IITMDSA-DTM11-Final-Project
# E-Commerce-Customer-Segmentation
This project aims to perform customer segmentation analysis on an E-commerce dataset using the K-means clustering algorithm. The goal is to identify the optimal number of clusters (k) based on the maximum silhouette score and uncover purchasing patterns among customers.

# Dataset Information:

The data was collected from a well known E-commerce website over a period of time based on the customer’s search profile.

# Variable Description:

* Column         -      Description
* Cust_ID        -      Unique numbering for customers
* Gender         -     Gender of the customer
* Orders         -      Number of orders placed by each customer in the past

Remaining 35 features (brands) contains the number of times
customers have searched them

# Work Flow

  * First Import the necessary libraries needed for the project. Below are the libraries that I have used
    
        > import pandas as pd
        > import numpy as np
        > import matplotlib.pyplot as plt
        > import seaborn as sns
        > from sklearn.preprocessing import MinMaxScaler
        > from sklearn.metrics import silhouette_score
        > from sklearn.cluster import KMeans
        > from yellowbrick.cluster import KElbowVisualizer
    
   * Load the dataset using pandas.
     
   * Understand the data with basic statistics, info, total records, features and their data types also number of null values.
     
   * Perform the data cleaning techniques like treating the missing values.
     
   * Visualize the data with the help of Matplotlib or Seaborn to get better understanding of the features.
     
       > In my project I have used Seaborn's,
       > Boxplot(To visualize the Outliers present in the data),
       > Barplot (To get to 10 customer ID based on Total searches),
       > Countplot (To get gender count and Prior orders count),
       > Heatmap (To find the Correlation),
       > Histogram (To get know how the data is distributed).
       
# CONCLUSION:

In E-commerce customer segmentation the k-Means clustering plays major role for identifying the purchase pattern based on customer interest ,Here I used silhoutte score for finding an optimal cluster number to predict the right n_cluster. After that I split the two types cluster 1 is previlge to moderate customer and cluster 0 is low-set of interest in purchasing
      
