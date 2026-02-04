# Customer Segmentation using K-means Clustering

This project performs customer segmentation using K-means clustering algorithm on retail transaction data. The goal is to analyze customer purchasing behavior and group customers into distinct segments based on their transaction patterns, helping businesses understand their customer base better and tailor marketing strategies accordingly.

## Project Overview

The project uses the Online Retail II dataset containing customer transactions from a UK-based online retail store. The dataset includes information about customer IDs, transaction dates, product details, quantities, and prices.

## Data Processing

The project follows a comprehensive data cleaning and preprocessing pipeline:

1. **Data Cleaning**: Handles missing values, removes invalid transactions, and processes outliers
2. **Feature Engineering**: Creates key customer metrics including:
   - **Monetary Value**: Total amount of money spent by each customer
   - **Frequency**: Total number of purchases made by each customer
   - **Recency**: Number of days since the last purchase
3. **Data Scaling**: Standardizes features using StandardScaler to ensure equal contribution to clustering

## Clustering Methodology

The project implements K-means clustering with the following approach:

1. **Optimal Cluster Selection**: Uses both Inertia and Silhouette Score metrics to determine the optimal number of clusters
2. **Cluster Analysis**: Identifies 4 main customer segments based on their purchasing behavior
3. **Outlier Handling**: Considers extreme customers separately for special attention

## Customer Segments

The project identifies four main customer segments:

1. **Retain**: High-value customers who purchase regularly
2. **Nurture**: New or less active customers with recent purchases
3. **Reward**: Most loyal customers with high frequency and value
4. **Re-Engage**: Infrequent buyers who need re-engagement

Additionally, the project identifies special outlier segments:
- **Pamper**: High spenders but not necessarily frequent buyers
- **Upsell**: Frequent buyers who spend less per purchase
- **Delight**: Most valuable customers with extreme spending and frequent purchases

## Technologies Used

- **Python 3.13**
- **Pandas** - Data manipulation and analysis
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical visualization
- **Scikit-learn** - Machine learning algorithms including K-means clustering
- **Jupyter Notebook** - Interactive development and analysis

## Project Files

- `customer-analysis-with-k-means-clustering.ipynb` - Main analysis notebook
- `requirements.txt` - Python dependencies
- `data/online_retail_II.xlsx` - Retail transaction dataset

## Getting Started

1. Clone the repository
2. Install dependencies using `pip install -r requirements.txt`
3. Run the Jupyter notebook to see the complete analysis
4. The notebook includes all data processing, clustering, and visualization steps

## Key Insights

The project provides actionable insights for each customer segment, helping businesses:
- Identify high-value customers for retention
- Target new customers for nurturing
- Reward loyal customers
- Re-engage inactive customers
- Handle special cases like high spenders and frequent buyers

This customer segmentation approach enables data-driven decision making for marketing strategies and customer relationship management.