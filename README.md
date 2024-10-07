# Customer Segmentation Using K-Means Clustering

## Overview
This project demonstrates the use of **K-Means clustering** to segment customers based on their **annual income** and **spending scores**. Customer segmentation is crucial for businesses to target their marketing efforts effectively by understanding customer behaviors and preferences. By categorizing customers into distinct groups, businesses can optimize their marketing strategies, personalize products or services, and improve customer engagement.

## Objective
The objective of this project is to apply the K-Means clustering algorithm to group customers into meaningful segments. These segments are based on their **annual income** and **spending score**, which helps businesses better understand the behavior of their customers and target their offerings accordingly.

## Dataset
The dataset used in this project contains information on 200 customers with the following features:
- **Customer ID**: Unique identifier for each customer.
- **Gender**: The gender of the customer (Male or Female).
- **Age**: Age of the customer.
- **Annual Income**: Annual income of the customer in thousands (k).
- **Spending Score**: The score assigned to the customer based on their spending habits.

### Example of the Dataset:
| CustomerID | Gender | Age | Annual Income (k$) | Spending Score (1-100) |
|------------|--------|-----|--------------------|------------------------|
| 1          | Male   | 19  | 15                 | 39                     |
| 2          | Female | 21  | 15                 | 81                     |
| 3          | Male   | 20  | 16                 | 6                      |

## Methodology
### 1. **Data Preprocessing**
- **Handling Missing Data**: Ensuring that there are no missing or null values in the dataset.
- **Feature Scaling and Normalization**: Scaling features like **annual income** and **spending score** to bring them to comparable ranges.
- **Categorical Encoding**: Converting categorical data (gender) into numerical values for the algorithm to process.

### 2. **Data Visualization**
- **Distribution Plots**: Visualizing the distribution of features like **age**, **annual income**, and **spending score**.
- **Count Plots**: Displaying the count of customers within different categories (e.g., age groups, income levels).
- **Heatmap**: Showing the correlations between variables (e.g., how income and spending score are related).

### 3. **K-Means Clustering**
- **Elbow Method**: Determining the optimal number of clusters by plotting the sum of squared distances (WCSS) and identifying the "elbow point."
- **K-Means Algorithm**: Applying the K-Means clustering algorithm to divide customers into distinct groups based on **annual income** and **spending scores**.

### 4. **Cluster Interpretation**
After running the K-Means algorithm, five clusters were identified:
- **Cluster 1**: Low Budget (low income, low spending).
- **Cluster 2**: Spenders (high income, high spending).
- **Cluster 3**: Average (moderate income and spending).
- **Cluster 4**: Savers (high income, low spending).
- **Cluster 5**: Best (high income, high spending).

## Results
The clustering results revealed five distinct customer segments, each representing different spending behaviors. Businesses can use this information to tailor their marketing strategies for each segment:
- **Spenders and Best**: Focus on premium products and high-end services.
- **Low Budget and Savers**: Offer discounts and promotions to encourage spending.

## Requirements
To run this project, you’ll need the following Python libraries:
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Matplotlib & Seaborn**: For data visualization.
- **Scikit-learn**: For implementing the K-Means clustering algorithm.

You can install the required libraries using:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
