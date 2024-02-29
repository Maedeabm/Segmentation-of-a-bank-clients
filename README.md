# Credit Card Segmentation using K-Means Clustering

This project demonstrates the use of K-means clustering to segment credit card users based on their usage patterns. The dataset contains various features related to credit card usage, such as balance, purchase frequency, cash advance frequency, etc.

## Libraries Used

- **Pandas**: For data manipulation and analysis.
- **Seaborn and Matplotlib**: For data visualization.
- **Scikit-learn**: For data preprocessing and clustering.
- **Yellowbrick**: For visualizing the elbow method to determine the optimal number of clusters.

## Data Preprocessing

- **Loading Data**: The credit card dataset is loaded into a Pandas DataFrame from a CSV file.
- **Cleaning Data**: The 'CUST_ID' column is dropped, and rows with missing values are removed to ensure data quality.
- **Feature Scaling**: The features are standardized using `StandardScaler` to ensure that the clustering algorithm treats all features equally.

## Exploratory Data Analysis (EDA)

- Descriptive statistics and a concise summary of the DataFrame are generated to understand the data's distribution and structure.
- Histograms for each feature are plotted to visualize their distributions.

## K-Means Clustering

- **Determining the Number of Clusters**: The elbow method is used to find the optimal number of clusters by plotting the within-cluster sum of squares (WCSS) against the number of clusters.
- **Clustering**: K-means clustering is applied to the scaled data with the chosen number of clusters.
- **Cluster Labels**: The cluster labels are assigned to each record in the original DataFrame.

## Cluster Analysis

- **Cluster Centers**: The centers of each cluster are calculated and transformed back to the original scale for interpretation.
- **Segmentation Visualization**: Histograms are plotted for each feature, colored by cluster labels, to visualize the segmentation.
- **Cluster Characteristics**: The mean values of each feature for each cluster are calculated and displayed to understand the characteristics of each cluster.

## Conclusion

The results of the K-means clustering provide insights into different segments of credit card users, which can be used for targeted marketing strategies, customer retention, and personalized services.
