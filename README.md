# Customer Segmentation Analysis 📊

This project performs **customer segmentation** using **K-Means** and **DBSCAN clustering algorithms** based on **Annual Income** and **Spending Score**. 🧑‍💻  
The analysis helps uncover meaningful customer groups for better marketing and personalization strategies.  

---

## ✨ Analysis Steps  

1. **Data Loading and Exploration** 🧐  
   - Loaded the `Mall_Customers.csv` dataset.  
   - Explored structure, summary statistics, and distributions.  

2. **Data Scaling** 📏  
   - Scaled **Annual Income (k$)** and **Spending Score (1-100)** using `StandardScaler` to ensure equal contribution in clustering.  

3. **K-Means Clustering** 🎯  
   - Used the **Elbow Method** to find the optimal number of clusters (**K = 5**).  
   - Applied K-Means with 5 clusters.  
   - Visualized clusters using scatter plots (Income vs Spending Score).  
   - Calculated **average spending score** for each cluster. 💰  

4. **DBSCAN Clustering** 🌌  
   - Applied DBSCAN to the scaled data.  
   - Identified clusters and noise points (-1).  
   - Visualized clusters with scatter plots.  
   - Calculated **average spending score** for DBSCAN clusters. 💵  

5. **Comparison of Results** 🤔  
   - Compared cluster structures and spending score averages between K-Means and DBSCAN.  

---

## 🔑 Key Findings  

- **K-Means (K = 5)**  
  - Average spending scores ranged from **17 to 82**, clearly differentiating spending behaviors. 🎯💰  
  - Clusters were **well-separated and circular**, suitable for distinct customer groups. 🔵🟢  

- **DBSCAN**  
  - Identified **3 clusters + noise points**.  
  - Average spending scores:  
    - Cluster 0 → ~43  
    - Cluster 1 → ~82.8  
    - Noise points (-1) → ~46.9 🌌  
  - Captured **irregular cluster shapes** and flagged outliers. 🌠  

---

## 📊 Visual Insights  

- **K-Means:** Clear separation into 5 customer groups based on average characteristics.  
- **DBSCAN:** Found dense regions and labeled sparse points as noise, revealing hidden structure.  

---

## 🤔 Insights / Next Steps  

- **K-Means** is useful for **fixed, well-defined customer segments**.  
- **DBSCAN** is better for **detecting irregular clusters and outliers**.  
- Deeper analysis using other attributes (e.g., **age, gender, family size**) could provide richer insights. 🧐  
- Identified customer segments can support:  
  - **Targeted marketing campaigns** 📈  
  - **Personalized customer experiences** 🛍️  

---

## 🚀 How to Run  

1. Clone this repository:  
   ```bash
   git clone https://github.com/your-username/customer-segmentation.git
   cd customer-segmentation
