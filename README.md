# 🧠 Unsupervised Learning – K-Means Clustering Project

In this project, I studied and applied the **K-Means Clustering** algorithm to a real-world retail dataset to segment customers based on their purchasing behavior.

---

## 📌 Problem Statement

Retailers often need to segment customers to:
- Understand purchasing behavior
- Personalize marketing strategies
- Identify high-value vs. low-value customers

In this project, I used **K-Means**, a popular unsupervised machine learning algorithm, to find natural groupings in customer data without predefined labels.

---

## 📊 Dataset Used

- Source: `Online Retail Dataset`
- Description: Contains transactional records of a UK-based online retailer over a period of time.
- Key fields used:
  - `CustomerID`
  - `Quantity`
  - `UnitPrice`
  - `InvoiceNo`
  - `InvoiceDate`

---

## 🔧 Steps Performed

1. **Data Cleaning**
   - Removed nulls and negative/zero quantity transactions.
   - Calculated `TotalPrice = Quantity × UnitPrice`.

2. **Feature Engineering**
   - Aggregated data by `CustomerID` to get:
     - `TotalPrice`: Total spend
     - `Quantity`: Total items bought
     - `NumPurchases`: Number of unique purchases

3. **Feature Scaling**
   - Used `StandardScaler` to normalize data for clustering.

4. **Optimal K Selection**
   - Applied **Elbow Method** and **Silhouette Score** to choose the best value for `k`.

5. **Clustering with K-Means**
   - Trained K-Means with the selected `k`.
   - Added `Cluster` labels to each customer.

6. **Evaluation & Visualization**
   - Visualized clusters in both 2D and 3D.
   - Achieved a **Silhouette Score of 0.95**, indicating strong clustering.
   - Interpreted and profiled each customer segment.

---

## 📘 Key Concepts (Revision Notes)

- **Unsupervised Learning**: Learning from data **without labels**. The algorithm finds hidden patterns or groupings.
- **K-Means Clustering**: Partitions data into `k` clusters based on feature similarity (minimizing intra-cluster distance).
- **Elbow Method**: Helps find the optimal `k` by plotting Within-Cluster Sum of Squares (WCSS).
- **Silhouette Score**: Evaluates how well each point fits in its cluster (`-1` to `1`; higher is better).
- **Feature Scaling**: Normalization is important for K-Means since it’s distance-based.

---

## 🧪 Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn (for plotting)
- Jupyter Notebook

---

## 📎 Outputs

- Clustered customers into meaningful groups (e.g., high-spenders, one-time buyers)
- Visual 2D & 3D plots of clusters
- Ready-to-use pipeline for future unsupervised ML projects

---

# Happy Learning

