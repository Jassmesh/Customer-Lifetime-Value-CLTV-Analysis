# 🧮 Customer Lifetime Value (CLTV) Analysis

## 📌 Introduction
Customer Lifetime Value (CLTV) is a predictive metric that estimates the total revenue a business can expect from a customer throughout their relationship. This project performs a data-driven CLTV analysis to help businesses prioritize high-value customers and optimize marketing efforts.

## 📄 Abstract
This analysis uses historical transaction data to compute CLTV for each customer using probabilistic models. The objective is to segment customers into distinct groups based on their predicted value, enabling better targeting strategies.

We apply BG/NBD and Gamma-Gamma models to estimate purchase frequency and average monetary value, respectively. The result is a ranked customer base segmented into tiers (A to D) for marketing actions.

## 🛠️ Tools Used
- **Python** – Main programming language
- **Pandas** – Data manipulation and cleaning
- **Matplotlib, Seaborn** – Data visualization
- **Lifetimes** – CLTV modeling (BG/NBD & Gamma-Gamma)
- **Jupyter Notebook** – Interactive development environment

## 🔧 Steps Involved in Building the Project

1. **Data Preprocessing**
   - Loaded transaction data
   - Removed canceled orders and missing values
   - Filtered data for valid transactions

2. **Feature Engineering**
   - Generated features: `recency`, `T`, `frequency`, and `monetary`
   - Aggregated data per customer

3. **Modeling**
   - Applied **BG/NBD model** to predict purchase frequency
   - Applied **Gamma-Gamma model** to predict average transaction value

4. **CLTV Calculation**
   - Estimated 6-month and 12-month CLTV
   - Created a final dataset containing customer CLTVs

5. **Customer Segmentation**
   - Divided customers into 4 segments (`A`, `B`, `C`, `D`) based on CLTV quartiles

6. **Visualization**
   - Plotted customer segments and CLTV distributions

## ✅ Conclusion
This CLTV model helps businesses identify and prioritize high-value customers, allocate resources efficiently, and design more effective marketing strategies. With accurate CLTV predictions, companies can improve customer retention and profitability.

---

## 📂 Repository Contents

- `CLTV_analysis.ipynb` –  Python notebook with full analysis
- `predicted_cltv.csv` - Final LTV prediction CSV
-                         Trained model + visualizations

