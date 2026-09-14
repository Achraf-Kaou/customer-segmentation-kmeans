# Customer Segmentation using RFM & K-Means Clustering

An end-to-end machine learning project that analyzes raw transaction data from an online retailer to group customers into distinct marketing personas based on their purchasing habits.

## 📊 Project Overview
By applying data science techniques, this project helps businesses understand their customer base. Instead of treating all shoppers the same, the model groups them so marketing teams can target them with tailored campaigns.

### Key Features Used (RFM Model)
* **Recency:** Days since the customer's last purchase.
* **Frequency:** Total number of unique orders placed.
* **Monetary Value:** Total cash spent by the customer.

## 🛠️ Tech Stack & Environment
* **Language:** Python 3
* **Environment:** Jupyter Notebook / Anaconda
* **Key Libraries:** Pandas, NumPy, Scikit-Learn (KMeans, StandardScaler), Matplotlib, Seaborn

## 🚀 Steps Executed
1. **Data Cleaning:** Removed missing Customer IDs and filtered out invalid negative values (`Quantity` and `UnitPrice` > 0).
2. **Feature Engineering:** Calculated individual RFM metrics from raw timestamped transactions.
3. **Feature Scaling:** Applied `StandardScaler` to normalize features on a fair playing field for distance-based math.
4. **Optimization:** Used the **Elbow Method** to discover the mathematically optimal number of customer groups ($K=3$).
5. **Clustering:** Deployed the **K-Means** algorithm to segment the audience.

## 📈 Customer Personas Discovered
Through clustering, the model successfully isolated three major corporate profiles:
1. **Ultra-Whales (Outliers):** A tiny handful of extreme bulk buyers responsible for massive transactional spikes.
2. **Core Spenders & VIPs:** Regular, loyal shoppers who consistently spend healthy amounts.
3. **Low-Value / Quiet Shoppers:** Dormant or one-time buyers clustered heavily near the bottom left of the spending scale.

## 💻 How to Run This Project
1. Clone this repository:
   ```bash
   git clone https://github.com
   ```
2. Ensure you have Anaconda installed.
3. Open `Customer_Segmentation_Project.ipynb` in Jupyter Notebook and run the cells.

---
Developed by [Your Name] - 2026
