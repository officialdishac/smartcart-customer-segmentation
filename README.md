# SmartCart Customer Segmentation

## 📌 Problem Statement
SmartCart currently applies uniform marketing strategies across all customers, leading to inefficient targeting and missed opportunities for personalization. This project segments customers based on purchasing behavior, engagement, and demographics using unsupervised learning. The goal is to identify meaningful customer groups for data-driven marketing and improved retention.

---

## 📊 Dataset Overview
- **Total Records:** 2240 customers  
- **Features:** Demographics, purchasing behavior, website activity, and campaign response  

### Key Feature Categories:
- **Demographics:** Age, Income, Education, Marital Status  
- **Spending:** Amount spent on various product categories  
- **Behavior:** Purchase frequency (web, store, catalog), web visits  
- **Customer Metrics:** Recency, complaints, campaign response  

---

## ⚙️ Project Workflow

### 1. Data Preprocessing
- Handled missing values and cleaned dataset  
- Removed irrelevant features  

### 2. Feature Engineering
- Created **Age** and **Customer Tenure**  
- Computed **Total Spending** and **Total Children**  
- Grouped categorical features  

### 3. Outlier Treatment
- Identified outliers using pairplots  
- Removed extreme values in **Income** and **Age**

### 4. Exploratory Data Analysis
- Correlation heatmap and relationship analysis  

### 5. Data Transformation
- One-hot encoding for categorical variables  
- Feature scaling using StandardScaler  

### 6. Dimensionality Reduction
- Applied **PCA** for 2D and 3D visualization  

### 7. Clustering
- **K-Means Clustering**  
- **Agglomerative Clustering**  
- Optimal clusters selected using:
  - Elbow Method  
  - Silhouette Score  

---

## 📈 Key Insights from EDA

- Income strongly correlates with total spending, indicating higher purchasing power drives revenue  
- High spenders engage across multiple channels (store, catalog, web)  
- Frequent website visitors are not necessarily high spenders  
- Customers with more children tend to spend less  

---

## 👥 Customer Segments

- **Cluster 0: Budget Family Shoppers**  
  Low income, low spending, high deal usage → *Target with discounts and family bundles*

- **Cluster 1: Affluent Loyal Customers**  
  High income, high spending, strong engagement → *Loyalty programs and premium offers*

- **Cluster 2: Price-Sensitive Single Households**  
  Low income, low spending, high browsing → *Discount-driven campaigns*

- **Cluster 3: High-Value Independent Customers**  
  High income, high spending, highly responsive → *VIP services and retention strategies*

---

## 🎯 Business Impact
- Enables **targeted marketing strategies** instead of generic campaigns  
- Helps identify **high-value customers for retention**  
- Improves **conversion rates and marketing ROI**  
- Supports **data-driven decision making**

---

## 🧠 Conclusion
This project successfully identified four distinct customer segments using clustering techniques. The results highlight clear differences in spending behavior, engagement, and demographics across groups. These insights allow SmartCart to shift from generic marketing to personalized strategies, improving customer retention and optimizing marketing efforts.

---

## 🛠️ Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- PCA (Dimensionality Reduction)  

---

## 📌 Future Improvements
- Deploy model using Streamlit or Flask  
- Automate cluster labeling  
- Integrate real-time customer data  
