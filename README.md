# Customer-Segmentation-Analysis

This project applies **Unsupervised Machine Learning** to identify distinct customer segments for a retail business. By analyzing customer behavior (Spending Score, Income, Frequency, etc.), the project creates actionable "Customer Personas" to guide targeted marketing strategies.

## The dataset consists of **1,000 customer records** with the following features:
* **Demographics:** Age, Gender, Income.
* **Behavioral:** Spending Score (1-100), Membership Years, Purchase Frequency.
* **Transactional:** Last Purchase Amount, Preferred Category.

* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn (KMeans, StandardScaler, PCA, LabelEncoder)
* **Visualization:** Matplotlib, Seaborn

##  Methodology

### 1. Data Preprocessing
* Handled missing values (if any).
* **Label Encoding:** Converted categorical variables (`Gender`, `Preferred Category`) into numeric formats.
* **Feature Scaling:** Applied `StandardScaler` to normalize features like Income (thousands) and Membership Years (single digits) so the model treats them equally.

### 2. Determining Optimal Clusters (The Elbow Method)
* Ran K-Means for k=1 to k=10.
* Analyzed the **Inertia** (WCSS) to find the "Elbow Point."
* **Result:** The optimal number of clusters was identified as **4**.

### 3. Model Training & Visualization
* Trained the **K-Means algorithm** with `n_clusters=4`.
* Applied **PCA (Principal Component Analysis)** to reduce the 6-dimensional data into a 2D Scatterplot for visualization.

##  Key Results & Insights

The analysis identified **4 unique customer segments**:

| Segment | Persona | Characteristics | Strategy |
| :--- | :--- | :--- | :--- |
| **0** | **Premium One-Timers** | Moderate Income, High Spend per visit. | Upsell expensive accessories & warranties. |
| **1** | **Loyal Athletes** | Long-term members, frequent `Sports` buyers. | Loyalty rewards & early access to new gear. |
| **2** | **Passive High Earners** | High Income but Low Spending Score. | Re-engagement campaigns & luxury vouchers. |
| **3** | **Active Shoppers** | High Spending Score, frequent `Grocery` buyers. | Subscription models & bulk-buy discounts. 

 Author
BISMA YB

LinkedIn: https://www.linkedin.com/in/bisma-yb

GitHub: https://github.com/BismaYB
