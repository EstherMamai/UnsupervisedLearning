# Customer Segmentation Using Clustering

## Project Overview
This project focuses on customer segmentation using various clustering techniques. The goal is to categorize customers into different groups based on demographic and financial data to better understand customer behavior and improve business decision-making.

## Dataset
The dataset contains customer information with the following attributes:
- **Sex**
- **Marital Status**
- **Age**
- **Education**
- **Income**
- **Occupation**
- **Settlement Size**

After preprocessing, the dataset is encoded and standardized for clustering analysis.

## Preprocessing Steps
1. **Handling Missing Values**: Any missing values were either imputed or removed.
2. **Encoding Categorical Variables**: Applied appropriate encoding (one-hot or label encoding) for categorical features.
3. **Feature Scaling**: Standardized numerical features such as `Age` and `Income` to ensure uniformity in clustering.
4. **Feature Engineering**: Created new meaningful features based on existing data.

## Clustering Algorithms Used
Different clustering techniques were implemented and evaluated:

### 1. **K-Means Clustering**
- Used the Elbow Method and Silhouette Score to determine the optimal number of clusters.
- Applied K-Means to segment customers into groups.

### 2. **Hierarchical Clustering**
- Created dendrograms to visualize cluster formation.
- Used Agglomerative Clustering with Ward’s linkage method.

### 3. **DBSCAN (Density-Based Clustering)**
- Identified clusters based on density and detected outliers.

### 4. **Gaussian Mixture Model (GMM)**
- Used probabilistic clustering to determine soft cluster memberships.

### 5. **Mean Shift Clustering**
- Automatically detected the number of clusters without predefined values.

## Model Evaluation
- **Silhouette Score**: Used to assess clustering performance.
- **Cluster Visualization**: Plotted clusters to understand distributions across different customer features.
- **Business Insights**: Interpreted clusters to derive actionable insights for marketing strategies and customer engagement.

## Key Findings
- **Gender Distribution**: 54.3% Male
- **Settlement Size**: 49.5% from small cities, 27.2% from mid-sized cities, 23.4% from big cities.
- **Marital Status**: 50.3% single, 49.6% married.
- **Education**: 69.3% graduate school, 14.6% university, 14.4% other/unknown.

## Tools & Technologies
- **Python** (pandas, numpy, sklearn, seaborn, matplotlib)
- **Jupyter Notebook**
- **scikit-learn** for clustering models

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/EstherMamai/customer-segmentation.git
   cd customer-segmentation
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the clustering notebook:
   ```bash
   jupyter notebook
   ```
   Open `customer_segmentation.ipynb` and execute the cells.

## Future Improvements
- Implement deep learning for customer behavior analysis.
- Integrate clustering results into a business intelligence dashboard.
- Explore supervised learning models for targeted marketing.
