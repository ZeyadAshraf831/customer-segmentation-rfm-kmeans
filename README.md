# Customer Segmentation using RFM Analysis & K-Means Clustering

## Overview

This project applies **RFM Analysis (Recency, Frequency, Monetary)** and **K-Means Clustering** to segment customers based on their purchasing behavior using a real-world e-commerce dataset. The resulting customer segments support targeted marketing strategies and improve customer relationship management.

---

## Dataset

* **Source:** Online Retail E-commerce Dataset
* **Transactions:** 541,909
* **Unique Customers:** 4,338

---

## Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Power BI

---

## Project Workflow

1. Data Cleaning

   * Removed missing values, duplicates, cancelled orders, and invalid transactions.

2. Feature Engineering

   * Calculated RFM metrics:

     * Recency
     * Frequency
     * Monetary

3. Data Preprocessing

   * Applied logarithmic transformation.
   * Standardized features using `StandardScaler`.

4. Optimal Cluster Selection

   * Determined the optimal number of clusters using the Elbow Method and Silhouette Score.

5. Customer Segmentation

   * Applied K-Means clustering to group customers with similar purchasing behavior.

6. Business Interpretation

   * Assigned meaningful business labels to each customer segment.

7. Visualization

   * Visualized customer segments using 3D plots and an interactive Power BI dashboard.

---

## Customer Segments

| Segment | Description                                                |
| ------- | ---------------------------------------------------------- |
| VIP     | High-value customers with recent and frequent purchases.   |
| Loyal   | Regular customers with consistent purchasing behavior.     |
| New     | Recently acquired customers with limited purchase history. |
| Lost    | Inactive customers with low spending and long recency.     |

---

## Results

| Segment | Customers | Average Monetary |
| ------- | --------: | ---------------: |
| VIP     |       713 |           $8,088 |
| Loyal   |     1,166 |           $1,802 |
| New     |       837 |             $557 |
| Lost    |     1,622 |             $341 |

---

## Power BI Dashboard

### Dashboard Highlights

* 4,338 unique customers
* 541,909 transactions analyzed
* 4 customer segments
* Average Monetary: **$2,048**
* Average Recency: **92 days**

The dashboard provides:

* Customer segment distribution
* RFM metric analysis
* Segment performance comparison
* Business insights for marketing decisions

> Add Power BI dashboard screenshots here.

---

## Business Value

The segmentation enables businesses to:

* Identify high-value customers for loyalty programs.
* Improve customer retention strategies.
* Design personalized marketing campaigns.
* Reactivate inactive customers.
* Support data-driven business decisions.

---

## Project Structure

```text
customer-segmentation-rfm/
│
├── customer_segmentation_rfm_kmeans.ipynb
├── data/
├── dashboard/
├── images/
├── README.md
└── requirements.txt
```

---

## Future Improvements

* Compare K-Means with DBSCAN and Hierarchical Clustering.
* Deploy the project as an interactive web application.
* Automate customer segmentation for new incoming transactions.
* Predict Customer Lifetime Value (CLV).
