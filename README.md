### Customer Segmentation Engine

#### Project Overview

I developed a **Customer Segmentation Engine** to group customers into distinct clusters based on their purchase history, enabling targeted marketing strategies. Using an e-commerce dataset, I applied data wrangling to preprocess the data, visualized customer patterns, and implemented a clustering algorithm to identify segments like "frequent buyers," "high spenders," or "occasional shoppers." This project demonstrates practical business value and technical proficiency.

#### Dataset

- **Source**: [Online Retail Dataset on UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/352/online+retail)
- **Details**: Contains transactional data from a UK-based online retailer (2010-2011), with columns like InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, and Country.
- **Download**:
    - Direct link: [Online Retail Excel File](https://archive.ics.uci.edu/ml/machine-learning-databases/00352/Online%20Retail.xlsx)
    - Save it as Online_Retail.xlsx in your working directory.
- **Size**: ~541,000 rows, ~25 MB.

#### Steps

1. **Data Wrangling**: Aggregate transactions into customer-level features (e.g., total spend, purchase frequency).
2. **Visualization**: Explore customer behavior with scatter plots and histograms.
3. **Machine Learning**: Use K-Means clustering to segment customers.

### Explanation

1. **Data Wrangling**:
    - Loads the Online_Retail.xlsx dataset and removes invalid entries.
    - Aggregates transactions by CustomerID to compute frequency, total spend, and average spend.
    - Scales features for clustering.
2. **Visualization**:
    - Scatter plot shows frequency vs. total spend to reveal customer patterns.
    - Histogram displays the distribution of total spend.
    - Clustered scatter plot visualizes the final segments.
3. **Machine Learning**:
    - Uses K-Means clustering to group customers into 4 segments.
    - Assigns descriptive labels (e.g., "High Spenders") and provides a summary.

---

### Running the Code

1. **Requirements**:
    - Install libraries: pip install pandas numpy matplotlib seaborn scikit-learn openpyxl.
    - Download Online_Retail.xlsx from the UCI link and place it in your working directory.
2. **Execution**:
    - Run in a Python environment (e.g., Jupyter Notebook or terminal).
    - Outputs include two initial plots, a clustered scatter plot, cluster summary, sample customers, and marketing recommendations.
