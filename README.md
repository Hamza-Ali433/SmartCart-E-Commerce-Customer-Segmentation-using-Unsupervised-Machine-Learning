# SmartCart: E-Commerce Customer Segmentation using Unsupervised Machine Learning

## Project Overview

Understanding customer behaviour is one of the biggest challenges for modern e-commerce businesses. Customers differ in their purchasing habits, spending capacity, engagement level, and responsiveness to marketing campaigns. Treating every customer the same often results in ineffective marketing, lower customer retention, and missed revenue opportunities.

This project develops an **AI-powered customer segmentation system** for **SmartCart**, an e-commerce company, using **Unsupervised Machine Learning**. By analyzing historical customer data, the system automatically groups customers with similar behaviour into meaningful clusters. These customer segments can then be used to design personalized marketing campaigns, improve customer satisfaction, increase sales, and optimize business decisions.

Instead of applying one marketing strategy to every customer, SmartCart can now understand **who its customers are, how they shop, and what type of marketing strategy is most effective for each group.**

---

# Problem Statement

SmartCart serves customers across multiple countries and has collected extensive customer information including demographics, purchase behaviour, website activity, and marketing campaign responses.

Although the company has access to rich customer data, it currently uses the same marketing strategy for every customer without understanding different purchasing patterns. This leads to:

* Inefficient marketing campaigns
* Low customer engagement
* Poor customer retention
* Missed opportunities to identify premium customers
* Unnecessary discounts offered to customers who would purchase anyway

The objective of this project is to discover hidden customer groups using clustering algorithms and provide business recommendations for each customer segment.

---

# Dataset Description

The dataset contains information for approximately **2,240 customers** with **22 customer attributes**.

The features include:

* Customer demographics
* Income
* Age
* Education
* Marital status
* Number of children
* Customer tenure
* Website visits
* Purchase history
* Store purchases
* Catalog purchases
* Web purchases
* Campaign responses
* Customer complaints
* Spending behaviour

The dataset contains both numerical and categorical variables describing each customer's interaction with the business.

---

# Objectives

The primary objectives of this project are:

* Clean and preprocess customer data
* Perform Exploratory Data Analysis (EDA)
* Engineer meaningful business features
* Reduce dimensionality using PCA
* Discover customer groups using clustering algorithms
* Profile each customer segment
* Recommend business strategies for every customer group

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* PCA (Principal Component Analysis)
* K-Means Clustering
* Agglomerative Hierarchical Clustering
* KneeLocator

---

# Project Workflow

## 1. Data Cleaning

The dataset was cleaned before clustering by:

* Handling missing values
* Removing unnecessary columns
* Treating outliers
* Checking duplicate records
* Correcting data types

---

## 2. Feature Engineering

Several new features were created to better represent customer behaviour, including:

* Customer Age
* Customer Tenure
* Total Spending
* Total Children
* Living Status
* Simplified Education Categories

These engineered features provide a better representation of customer lifestyle and purchasing behaviour.

---

## 3. Data Preprocessing

Before clustering:

* Categorical variables were encoded
* Numerical features were standardized using **StandardScaler**
* The dataset was prepared for dimensionality reduction

---

## 4. Exploratory Data Analysis (EDA)

Several visualizations were created to better understand the dataset, including:

* Distribution plots
* Correlation heatmap
* Pair plots
* Customer spending analysis
* Income analysis
* Purchase behaviour visualization
* Cluster distribution

EDA helped identify relationships between customer income, spending behaviour, website activity, and campaign responses.

---

## 5. Principal Component Analysis (PCA)

Since the dataset contains many correlated features, PCA was applied to reduce dimensionality while preserving most of the information.

PCA was also used to visualize customer clusters in both **2D** and **3D** space.

---

## 6. Finding the Optimal Number of Clusters

The optimal number of clusters was determined using the **Elbow Method** and **KneeLocator**.

The analysis suggested:

**Optimal Number of Clusters = 4**

---

## 7. Clustering Algorithms

Two clustering techniques were implemented:

* K-Means Clustering
* Agglomerative Hierarchical Clustering

The resulting clusters were visualized using PCA components to better understand customer separation.

---

# Customer Segments

After analyzing the clusters, four distinct customer groups were identified.

---

# Cluster 0 — Family Budget Shoppers

### Characteristics

* Low to moderate income
* Low spending
* Higher number of children
* Mostly living with partners
* Lower campaign response
* High website activity
* Lower purchase frequency

### Business Insight

These customers frequently browse products but purchase less often. Their buying behaviour suggests they are price-sensitive and usually look for better deals before making purchases.

### Recommended Strategy

* Family discount bundles
* Coupon campaigns
* Seasonal promotions
* Buy-One-Get-One offers
* Affordable product recommendations

**Business Goal**

Increase conversion rate by encouraging website visitors to complete purchases.

---

# Cluster 1 — Loyal Premium Customers

### Characteristics

* High income
* High total spending
* High catalog purchases
* High in-store purchases
* Low website visits
* Mostly living with partners
* Strong purchasing behaviour

### Business Insight

These customers already trust the brand and consistently make purchases. They generate significant revenue and require retention rather than discounts.

### Recommended Strategy

* Loyalty reward programs
* VIP membership
* Exclusive product launches
* Personalized recommendations
* Premium customer support

**Business Goal**

Increase customer lifetime value and strengthen customer loyalty.

---

# Cluster 2 — Digital Window Shoppers

### Characteristics

* Lowest income group
* Lowest spending
* Highest website visits
* Few purchases
* Mostly living alone
* Moderate campaign response

### Business Insight

These customers spend considerable time browsing products but often leave without making purchases. They represent a strong opportunity for improving conversion rates.

### Recommended Strategy

* Flash sales
* First-order discounts
* Cart abandonment reminders
* Free shipping offers
* Limited-time promotional campaigns

**Business Goal**

Convert frequent website visitors into active customers.

---

# Cluster 3 — High-Value Elite Customers

### Characteristics

* High income
* Highest spending
* Highest campaign response
* Mostly living alone
* Long customer relationship
* Excellent purchasing behaviour

### Business Insight

This segment represents SmartCart's most valuable customers. They contribute significantly to revenue and respond well to marketing campaigns.

### Recommended Strategy

* Premium membership
* Exclusive collections
* Personalized shopping experience
* Luxury product recommendations
* Cross-selling and upselling
* Dedicated customer support

**Business Goal**

Retain high-value customers while maximizing their lifetime value.

---

# Business Recommendations

Based on the customer profiles, SmartCart should avoid using a single marketing strategy for every customer.

| Customer Segment           | Recommended Strategy                                            |
| -------------------------- | --------------------------------------------------------------- |
| Family Budget Shoppers     | Discounts, bundle offers, family promotions                     |
| Loyal Premium Customers    | Loyalty rewards, VIP membership, exclusive launches             |
| Digital Window Shoppers    | Flash sales, coupons, cart reminders, free shipping             |
| High-Value Elite Customers | Premium services, personalized recommendations, luxury products |

---

# Visualizations Included

The project contains several visualizations to understand customer behaviour and clustering results:

* Correlation Heatmap
* Pair Plot
* PCA 2D Visualization
* PCA 3D Visualization
* Elbow Method
* Cluster Distribution
* K-Means Cluster Visualization
* Agglomerative Cluster Visualization

---

# Key Outcomes

* Successfully segmented customers into four meaningful groups.
* Identified high-value customers for premium services.
* Identified price-sensitive customers for targeted discounts.
* Distinguished loyal customers from occasional browsers.
* Generated actionable marketing recommendations based on customer behaviour.
* Demonstrated how unsupervised learning can support real business decision-making.

---

# Conclusion

This project demonstrates how unsupervised machine learning can transform raw customer data into actionable business insights. By combining data preprocessing, feature engineering, PCA, and clustering techniques, SmartCart can better understand its customers and replace generic marketing campaigns with personalized strategies.

The resulting customer segments provide a practical foundation for targeted promotions, loyalty programs, premium services, and customer retention initiatives. Implementing these recommendations can help SmartCart improve marketing efficiency, increase customer satisfaction, and maximize long-term business value.
