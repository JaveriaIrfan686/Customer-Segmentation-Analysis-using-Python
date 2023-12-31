# Customer-Segmentation-Analysis-using-Python
The 'Mall_Customer' Dataset is from Kaggle. Its purpose is to get to know expenditure of customer based on certain parameters that are already declared in dataset.

# Preprocessing
For preprocessing, I have first checked details of the dataset by using anf info() and describe() method. The describe method prints the count, mean, standard deviation, min, max as they provide a summary of the central tendency, 
variability, and distribution of the data. Along with, I checked distribution of gender and female exceeds than male in terms of spending. Then I standarize the feature to ensures that all features have a consistent scale, making it 
easier to compare and analyze them.

# Elbow Method
I used elbow method to find out the best number of clusters. Point to be noted here is that the optimized number of cluster does not gaurantee best accuracy score of it. By the help of its graph, I analyzed that 5 number of clusters 
will be highlty optimized.

# K mean clustering
By using number of optimized cluster, analyzed from the graph of elbow method that is 5. I used this to find k mean clustering and print their centroid. Lets discuss its results:
  * ## Cluster 1 (Center [55.3, 49.5]):
       Customers in this cluster have moderate annual income and spending scores.
  * ## Cluster 2 (Center [86.5, 82.1]):
       Customers in this cluster have high annual income and high spending scores, likely representing high-value customers.
  * ## Cluster 3 (Center [25.7, 79.4]):
       Customers in this cluster have low annual income but high spending scores, possibly indicating price-insensitive shoppers.
  * ## Cluster 4 (Center [88.2, 17.1]):
       Customers in this cluster have high annual income but low spending scores, possibly representing frugal customers.
  * ## Cluster 5 (Center [26.3, 20.9]):
       Customers in this cluster have low annual income and low spending scores, likely representing budget-conscious shoppers.
    # Performance
      I checked the performance by using 2 methods that are:
       ## Silhouette Score
           Its score is 0.55, which generally considered a reasonable and acceptable score for clustering. This shows on average, the data points within each cluster are somewhat closer to each other than to data points in neighboring clusters. This suggests that the clusters have moderate cohesion (data points within clusters are similar) and separation (clusters are distinct from each other).
      ## Davies-Bouldin Index (DBI)
          Its score is 0.57, which indicates that my clusters are relatively well-separated and distinguishable. The fact that the index is significantly lower than 1 suggests that the clusters have a reasonable degree of separation. It demonstrates the ability to effectively analyze and structure our data. It suggests that we've captured meaningful relationships between data points while creating the clusters.
