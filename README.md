
# 🧠 RFM Customer Segmentation Analysis

This project performs **Customer Segmentation using RFM (Recency, Frequency, Monetary) Analysis** on real e-commerce transactional data. The goal is to help businesses identify high-value customers and tailor their marketing strategies accordingly.

---

## 📊 Dataset

- **Source**: [Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/online+retail)
- **Size**: ~500,000 transactions from a UK-based online retailer
- **Columns used**:  
  `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`

---

## 📌 Objectives

- Clean and preprocess customer transaction data
- Calculate **Recency**, **Frequency**, and **Monetary** values per customer
- Assign **RFM Scores** and generate **segments** like:
  - 🏆 Champion
  - 💰 Big Spender
  - ❤️ Loyal
  - ⚠️ At Risk
  - 🔍 Others
- Visualize customer distribution across segments

---

## 🛠️ Key Steps

1. **Data Cleaning**  
   - Removed null Customer IDs  
   - Filtered out canceled transactions (InvoiceNo starting with 'C')  
   - Added `TotalPrice` = `Quantity × UnitPrice`

2. **RFM Metrics Calculation**  
   - Recency = Days since last purchase  
   - Frequency = No. of unique purchases  
   - Monetary = Total revenue per customer

3. **Scoring**  
   - Assigned scores from 1–5 for each R, F, M metric  
   - Combined into an `RFM_Segment` (e.g., `555`) and `RFM_Score` (sum)

4. **Segmentation**  
   - Customers grouped into key segments using conditional logic

5. **Visualization**  
   - Bar chart and pie chart to show distribution of customer segments

---

## 📈 Visual Insights

### ▶ Segment Distribution (Pie Chart)

![Customer Segment Distribution]
<img width="578" height="470" alt="Customer_Segment_Pie" src="https://github.com/user-attachments/assets/2db0602d-2979-44f4-a643-473de365a764" />

- Majority fall under "Others"
- Champions, Loyal, and At-Risk customers represent key marketing targets

---

## 🔍 Business Value

This segmentation helps businesses:
- Target **loyal customers** with reward programs
- Re-engage **at-risk customers** with win-back campaigns
- Identify **big spenders** and **champions** for upselling opportunities

---

## 📁 Files in this Repo

- `RFM_Project.ipynb` – full analysis notebook
- `RFM_Customer_Segmentation.xlsx` – cleaned RFM export
- `Customer_Segment_Pie.png` – pie chart image (optional)
- `README.md` – project documentation

---

## 👩‍💻 Built With

- Python 🐍
- Pandas & NumPy
- Matplotlib
- Jupyter Notebook

---

## 📬 Let's Connect

If you like this project or want to collaborate, feel free to connect on [LinkedIn](https://www.linkedin.com/in/aishwarya-chintaluru-6797732bb/)
