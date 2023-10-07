# Geospatial-Data-Analysis-K-Means-Clustering-of-Latitude-and-Longitude-Data

This repository contains code and instructions for performing geospatial data clustering using K-Means clustering. We explore a dataset containing latitude and longitude information and aim to find meaningful clusters in the data.

## Workflow

1. **Data Preparation**
   - The initial dataset includes various columns, but for our analysis, we extracted and focused solely on the 'latitude' and 'longitude' data.

2. **2D Visualization**
   - We started by creating a simple 2D scatter plot to visualize the data points in latitude and longitude space. This helped us get a rough idea of the clusters' distribution but didn't provide a precise estimation of the optimal number of clusters.

3. **Elbow Method for Cluster Estimation**
   - To determine the optimal number of clusters (k), we employed the Elbow Method. This involved running K-Means with different values of k and plotting the within-cluster sum of squares (WCSS) or inertia. The "elbow point" on the graph, where the rate of change of inertia starts to slow down, was used as an estimate for the optimal k.

4. **Data Normalization**
   - We normalized the latitude and longitude data to have a mean of zero and a standard deviation of one using StandardScaler. This step is crucial to ensure that both latitude and longitude contribute equally to the clustering process.

5. **K-Means Clustering**
   - Based on the optimal k determined in step 3, we performed K-Means clustering on the normalized data. Each data point was assigned to one of the clusters based on its proximity to the cluster centroids.

6. **Cluster Visualization**
   - We visualized the results of the K-Means clustering by creating a scatter plot of latitude and longitude data, where each data point was colored according to its assigned cluster. This visualization allowed us to see how the data was grouped into clusters.

## Solutions and Insights

- By following the workflow described above, we were able to identify meaningful clusters within the geospatial data.
- The Elbow Method helped us estimate the optimal number of clusters, providing a balance between model complexity and data fit.
- The cluster visualization allowed us to observe the spatial distribution of the clusters, which can be valuable for further analysis or decision-making.

Feel free to use the code and adapt it for your own geospatial clustering tasks. Adjust the parameters and explore different datasets to gain insights from your data.
