# Customer Segmentation Assignment

## Overview
This project performs customer segmentation using clustering techniques on a dataset containing customer profiles and transaction information. The goal is to identify distinct customer segments based on their purchasing behavior and demographic information.

## Contents
- `Customers.csv`: Contains customer demographic information.
- `Transactions.csv`: Contains transaction details for each customer.
- `EDA.ipynb`: Jupyter Notebook containing the code for data preparation, clustering, and visualization.
- `Lookalike.csv`: Output file containing lookalike recommendations (if applicable).
- `README.md`: This README file.

## Requirements
To run this project, you will need the following Python packages:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`



## Data Preparation
The analysis is conducted using two datasets:

- **Customers.csv**: Contains demographic information such as CustomerID, Name, SignupDate, and Region.
- **Transactions.csv**: Contains transaction details such as TransactionID, CustomerID, ProductID, TransactionDate, Quantity, and TotalValue.

### Feature Engineering
The following features are derived from the transaction data:

- **Total Transactions**: The total number of transactions made by each customer.
- **Total Spending**: The total amount spent by each customer.
- **Average Transaction Value**: The average value of transactions.
- **Recency**: The number of days since the last transaction.

## Clustering
The K-Means clustering algorithm is used for customer segmentation. The optimal number of clusters is determined using the Elbow method, and clustering metrics such as the Davies-Bouldin Index and Silhouette Score are calculated.

### Results
- **Number of Clusters Formed**: 4
- **Davies-Bouldin Index**: 0.45
- **Silhouette Score**: 0.35

### Visualizations
Several visualizations are created to illustrate the clustering results:

- Elbow Method Plot
- Pair Plot of Customer Features
- 3D Scatter Plot of Clusters

## Running the Code
To run the analysis, open the files in Jupyter Notebook in your preferred environment (e.g., Jupyter Notebook, JupyterLab, or Google Colab). Execute the cells sequentially to perform data preparation, clustering, and visualization.

## Conclusion
This project successfully identifies distinct customer segments based on their transaction behavior and demographic information. The clustering metrics indicate that the segments are reasonably well-defined, and the visualizations provide valuable insights into the characteristics of each segment.
