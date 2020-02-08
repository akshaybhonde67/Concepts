K-Means Clustering- Get a meaningful intuition of the structure of the data we’re dealing with. Unsupervised, it groups similar data points together and discover underlying patterns. K-means algorithm is an iterative algorithm that tries to partition the dataset into K pre-defined distinct non-overlapping subgroups (clusters) where each data point belongs to only one group.<br>

Working<br>
1. Specify the number of clusters K.<br>
2. Initialize centroids by first shuffling the dataset and then randomly selecting K data points for the centroids without replacement.<br>
3. Compute the sum of the squared distance between data points and all centroids.<br>
4. Assign each data point to the closest cluster (centroid).<br>
5. Compute the centroids for the clusters by taking the average of all data points that belong to each cluster.<br>
6. Keep iterating until there is no change to the centroids. i.e assignment of data points to clusters isn’t changing.<br>
It halts creating and optimizing clusters when either: The defined number of iterations has been achieved or centroids dont change<br>

Problem<br>
Since k means algorithm may be stuck in a local optimum and may not converge to global optimum. <br>

Solution<br>
Therefore, it’s recommended to run the algorithm using different initializations of centroids and pick the results of the run that yielded the lower sum of squared distance.<br>

Validation method- Elbow method, Silhouette Score<br>
Elbow method - One commonly used approach is testing different numbers of clusters and measure the resulting sum of squared errors, choosing the K value at which an increase will cause a very small decrease in the error sum, while a decrease will sharply increase the error sum. This point that defines the optimal number of clusters is known as the “elbow point”, and can be used as a visual measure to find the best pick for the value of K.<br>


Silhouette analysis can be used to determine the degree of separation between clusters. For each sample: Compute the average distance from all data points in the same cluster (ai). Compute the average distance from all data points in the closest cluster (bi).<br>

The coefficient can take values in the interval [-1, 1].<br>
If it is 0 –> the sample is very close to the neighboring clusters.<br>
It it is 1 –> the sample is far away from the neighboring clusters.<br>
It it is -1 –> the sample is assigned to the wrong clusters.<br>
Therefore, we want the coefficients to be as big as possible and close to 1 to have a good clusters. Good n_clusters will have a well above 0.5 silhouette average score as well as all of the clusters have higher than the average score.<br>

Advantage- If variables are huge, then K-Means most of the times computationally faster, if we keep k smalls. 2) K-Means produce tighter clusters t K-Means <br>
Disadvantage- Slight variation in data can lead to high variance(very sensitive to outliers and noise), Difficult to predict K-Value, sensitive to local optimals.<br>

Assumption: Additionally, it assumes that data points in each cluster are modeled as located within a sphere around that cluster centroid (spherical limitation), but when this condition (or any of the previous ones) is violated, the algorithm can behave in non-intuitive ways. It tries to find centroids with neat spheres of data around them, and performs badly as the cluster’s geometric shape deviates from a sphere. It’s interesting to see that K-means doesn’t allow data points that are far away from each other to share the same cluster, no matter how obvious the relation between these data points might be.<br>

Application<br>
market segmentation, document clustering, image segmentation and image compression<br>
An example of that is clustering patients into different subgroups and building a model for each subgroup to predict the probability of the risk of having a heart attack.
