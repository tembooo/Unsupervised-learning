## K-Means Clustering Task

Implement a function for clustering given data using the k-means algorithm.  
The function call could look like this:

![image](https://github.com/user-attachments/assets/e0b4e1c4-0c71-458f-993d-72a834f25a82)

```python
[centers, assignments] = kmeans(data, k, epsilon)
```
Parameters and Outputs
data: contains the training samples

k: the number of clusters

epsilon: an optional difference threshold for continuing iteration

centers: a matrix containing the cluster centers

assignments: a vector of the length as the number of samples, specifying which cluster each sample was assigned to

Let us assume that the given data with 100 samples contains 2 to 5 clusters.
Experiment with the k-means algorithm to cluster the provided data.
Use squared Euclidean distances as a metric. Quantitatively select an optimal value for k based on the mean of silhouette values
(the higher the silhouette score, the better the clustering quality).
You can use implementations from existing libraries.

Based on this criterion:
The optimal value for k is: 2

The sum of squared Euclidean distances from all the samples to their assigned centroids is: 153.239

Additional Files
CSV, MAT

Hints
Set the random number generator seed to the default value for reproducibility.

Initialise the centroids uniformly from the range of the data.

Perform 10 iterations for each number of clusters (to avoid the potential problem of initialisation).

MATLAB: Use the silhouette function to calculate silhouette values.

Python: Use silhouette_score from sklearn.metrics:

from sklearn.metrics import silhouette_score


---

Let me know if you'd like to append this directly into a full project README with headers.

