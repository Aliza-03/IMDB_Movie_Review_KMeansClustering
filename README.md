# Movie Review Clustering Using KMeans
This project implements K-means clustering from scratch to group movies based on their ratings and analyzes how well movie genres align within clusters. The project uses the **IMDB Movie Dataset** from Kaggle and clusters the movies into three categories: `Top Rated`, `Average Rated`, and `Low Rated`. 
We then evaluate how these clusters correlate with movie genres.

## Dataset

The dataset used is **IMDB-Movie-Data.csv**, which contains:
- **Rating**: Movie rating (out of 10).
- **Votes**: Number of votes the movie received.
- **Revenue (Millions)**: Movie's revenue in millions.
- **MetaScore**: Score from Metacritic.
- **Year**: The release year of the movie.
- **Genre**: The genre(s) of the movie.

- ## Objective

The goal of this assignment is to:
1. **Cluster movie reviews based on ratings** using K-means clustering.
2. **Analyze whether movies within the same rating clusters belong to similar genres.**
3. **Evaluate** the clustering results using a confusion matrix.
4. **Visualize the clusters** using 2D and 3D scatter plots.

### Rating Clusters

- **Top Rated**: Movies with a rating of 8 or above.
- **Average Rated**: Movies with a rating between 6 and 7.9.
- **Low Rated**: Movies with a rating below 6.

  ### 2. K-means Clustering Implementation

We implement K-means clustering from scratch using Numpy. The algorithm involves:
- **Centroid Initialization**: Randomly initializing three centroids.
- **Cluster Assignment**: Assigning each movie to the nearest centroid.
- **Centroid Update**: Recomputing the centroid as the mean of all points in a cluster.
- **Convergence Check**: The algorithm stops when centroids no longer change.

### 3. Genre Analysis

After clustering the movies, we analyze whether movies within the same cluster share similar genres. We also evaluate the clustering performance by comparing the clusters with the original rating-based categories using a **confusion matrix**.
![image](https://github.com/user-attachments/assets/635988ba-3aae-4bdb-b72d-ffd94976ecb8)

### 4. Visualization

We generate both **2D and 3D visualizations** to display the clusters:
- **2D Scatter Plot**: Movies are plotted by `Rating` vs. `Votes`, with clusters colored differently.
  ![image](https://github.com/user-attachments/assets/ccac1112-109d-4100-992e-e06540f77327)
