# DSND_Identify_Customer_Segments
### Project Overview

In this project, I applied unsupervised learning techniques to identify segments of the population that form the core customer base for a mail-order sales company in Germany. These segments can then be used to direct marketing campaigns towards audiences that will have the highest expected rate of returns. The data that you will use has been provided by our partners at Bertelsmann Arvato Analytics, and represents a real-life data science task.  

2. - ### Project Components

     This Jupyter Notebook contains following steps: 

     1. Load the data:

        There are four files associated with this project (not including this one):

        - `Udacity_AZDIAS_Subset.csv`: Demographics data for the general population of Germany; 891211 persons (rows) x 85 features (columns).
        - `Udacity_CUSTOMERS_Subset.csv`: Demographics data for customers of a mail-order company; 191652 persons (rows) x 85 features (columns).

        Each row of the demographics files represents a single person, but also includes information outside of individuals, including information about their household, building, and neighborhood.

     2. Preprocessing

        -  Accessing Missing Data
        - Re-Encode Features
        - Feature Transformation
          - Feature scaling using StandardScaler
          - Using Imputer to replace missing values.
        - Dimensionality Reduction
          - Use sklearn's PCA class to apply principal component analysis on the data, thus finding the vectors of maximal variance in the data. 
          - Check out the ratio of variance explained by each principal component as well as the cumulative variance explained.

     3. Clustering

        - Use sklearn's KMeans class to perform k-means clustering on the PCA-transformed data.
        - Compute the average difference from each point to its assigned cluster's center.
        - Perform the above two steps for a number of different cluster counts.
        - Selected a final number of clusters to use, re-fit a KMeans instance to perform the clustering operation.

     

     