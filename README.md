# Customer Segmentation using K-means Clustering

A data science project that performs customer segmentation using K-means clustering algorithm on retail transaction data.

## Project Overview

This project analyzes customer purchasing behavior and segments customers into distinct groups based on their transaction patterns. The segmentation helps businesses understand their customer base better and tailor marketing strategies accordingly.

## Features

- **Data Cleaning**: Handles missing values, removes invalid transactions, and processes outliers
- **Feature Engineering**: Creates key customer metrics including Monetary Value, Frequency, and Recency
- **Clustering**: Implements K-means clustering with optimal cluster selection using Silhouette Score
- **Visualization**: Provides 3D scatter plots and distribution charts for cluster analysis
- **Customer Insights**: Generates actionable insights for each customer segment

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd customer-segmentation-using-k-means
```

2. Create and activate virtual environment:
```bash
python -m venv venv
venv\Scripts\activate  # On Windows
source venv/bin/activate  # On macOS/Linux
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Place your data file in the `data/` directory
2. Update the file path in the notebook if needed
3. Run the Jupyter notebook:
```bash
jupyter notebook customer-analysis-with-k-means-clustering.ipynb
```

## Project Structure

```
customer-segmentation-using-k-means/
├── .gitignore              # Git ignore rules
├── README.md               # This file
├── requirements.txt        # Python dependencies
├── customer-analysis-with-k-means-clustering.ipynb  # Main analysis notebook
├── data/                   # Data files (ignored by git)
│   └── online_retail_II.xlsx
└── venv/                   # Virtual environment (ignored by git)
```

## Key Insights

The project identifies four main customer segments:
- **Retain**: High-value customers who purchase regularly
- **Nurture**: New or less active customers with recent purchases
- **Reward**: Most loyal customers with high frequency and value
- **Re-Engage**: Infrequent buyers who need re-engagement

## Technologies Used

- **Python 3.13**
- **Pandas** - Data manipulation
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical visualization
- **Scikit-learn** - Machine learning algorithms
- **Jupyter Notebook** - Interactive development

## License

This project is licensed under the MIT License.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request