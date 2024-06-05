# E-Commerce Customer Segmentation using RFM Analysis
Project Overview

This project aims to analyze and segment the customers of an e-commerce website using the RFM (Recency, Frequency, Monetary) approach. The goal is to enable the company to optimize retention and acquisition strategies. The analysis was performed using Python in Jupyter Notebook, and K-means clustering was used for segmentation.
Dataset

The dataset consists of customer transactions from an e-commerce website. Key features include:

    CustomerID: Unique identifier for each customer.
    Item Code: Unique code for each item.
    InvoiceNo: Unique invoice number for each transaction.
    Date of purchase: The date when the order was placed.
    Quantity: Number of items purchased.
    Time: Time of the purchase.
    Price per Unit: Price per unit of the item.
    Price: Total amount spent on each transaction.
    Shipping Location: Location where the order was shipped.
    Cancelled_status: Indicates if the order was canceled.
    Reason of return: Reason for returning the item (if any).
    Sold as set: Indicates if the item was sold as part of a set.

Methodology

    Data Cleaning:
        Handling Missing Values: Dropped rows with missing CustomerID as it's crucial for grouping and calculating RFM metrics.
        Date and Time Processing: Converted Date of purchase to datetime format and extracted necessary time-related features.
        Data Filtering: Removed canceled transactions and irrelevant columns for RFM analysis.

    RFM Segmentation:
        Recency: Calculated as the number of days since the last purchase.
        Frequency: Total number of purchases per customer.
        Monetary: Total amount spent by each customer.

    K-means Clustering:
        Optimal Clusters: Determined the optimal number of clusters using the elbow method.
        Clustering: Applied K-means clustering to segment customers into different groups.

Results

The final segmentation results are as follows (average values for each cluster):

    Cluster 1 (29% of customers):
        Recency: 20 days
        Frequency: 230 purchases
        Monetary: $764 million

    Cluster 2 (31% of customers):
        Recency: 64 days
        Frequency: 57 purchases
        Monetary: $160 million

    Cluster 3 (22% of customers):
        Recency: 126 days
        Frequency: 24 purchases
        Monetary: $50 million

    Cluster 4 (18% of customers):
        Recency: 220 days
        Frequency: 10 purchases
        Monetary: $10 million

Interpretation

    Cluster 1: Highly active and high-spending customers. Priority for retention and high-value promotions.
    Cluster 2: Moderately active with significant spending. Target for regular engagement and upselling.
    Cluster 3: Less active with lower spending. Potential for reactivation campaigns.
    Cluster 4: Least active and low-spending customers. Focus on cost-effective engagement strategies.

Conclusion

This project demonstrates the use of RFM analysis and K-means clustering to segment customers effectively. The insights derived can help the e-commerce company tailor its marketing strategies to different customer segments, enhancing customer satisfaction and business performance.
