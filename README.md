# Iris Dataset Clustering with K-Means
This code demonstrates the application of K-Means clustering algorithm on the famous Iris dataset. The Iris dataset is a multivariate dataset that consists of measurements of sepal length, sepal width, petal length, and petal width for three different species of iris flowers: Setosa, Versicolour, and Virginica.

The code is written in Python and utilizes popular libraries such as NumPy, Matplotlib, Pandas, Seaborn, and Scikit-learn.

# Code Overview
1. Data Loading and Exploration:

The code starts by importing the necessary libraries and loading the Iris dataset using Scikit-learn's datasets module.
The dataset is then converted into a Pandas DataFrame for easier manipulation and exploration.
Various exploratory methods such as .head(), .info(), .describe(), and .shape are used to gain insights into the dataset.

2. Data Visualization:

The code utilizes Seaborn to create visualizations of the dataset. It includes pairplots, which show pairwise relationships between the features, and a heatmap, which displays the correlation between the features using color-coded annotations.

3. Applying the Elbow Method:

The Elbow Method is used to determine the optimal number of clusters for K-Means. It calculates the Within-Cluster Sum of Squares (WCSS) for different numbers of clusters (ranging from 1 to 10) and plots the Elbow Curve.
The plot helps to identify the "elbow" point, which indicates the number of clusters that provides a good balance between compactness and separation.

4. K-Means Clustering:

K-Means clustering is applied to the dataset using Scikit-learn's KMeans class. The optimal number of clusters determined from the Elbow Method (3 clusters) is used.
The code assigns cluster labels to each data point and visualizes the clusters using scatter plots. Each species of iris flower is represented by a different color, and the centroids of the clusters are also displayed.

5. Cluster Analysis:

The cluster labels are mapped to the original target names ('Iris-setosa', 'Iris-versicolour', 'Iris-virginica') for better interpretation.
A new DataFrame is created with the cluster labels added as a new column.
The code generates visualizations to analyze the distribution of each feature within each cluster using violin plots.
Additionally, a pairplot is created to visualize the relationships between variables within each cluster.

# Conclusion

This code provides a comprehensive example of applying K-Means clustering to the Iris dataset. By visualizing the clusters and analyzing the distribution of features within each cluster, it helps in understanding the natural groupings present in the data.

Feel free to modify the code and experiment with different clustering algorithms, feature combinations, or dataset visualizations to gain deeper insights into the Iris dataset or apply clustering techniques to other datasets.
