# 💳 PayWave Transactions 2024  
### Data Analysis & Visualization Project

## 📌 Project Description
This project focuses on analyzing PayWave transaction data from 2024 using Python for data cleaning, exploratory data analysis (EDA), and visualization.

The analysis aims to uncover:
- Transaction trends over months
- Markets generating the most transactions
- Merchants generating the highest revenue
- Fraud/flagged transaction patterns
- Payment methods performance

---

# 🛠️ Tools & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

# 📂 Dataset

Dataset used:
- `paywave_transactions_2024.csv`

Key columns analyzed:
- Date
- Market
- Merchant
- Amount_USD
- Fee_USD
- Payment_Type
- Fraud_Flag

---

# 🧹 Data Cleaning Process

The following cleaning steps were performed:

- Converted `Date` column into datetime format
- Checked for duplicate values
- Checked for missing values
- Created ordered monthly categories for trend analysis

Example:
```python
df["Date"] = pd.to_datetime(df["Date"])
```

---

# 📊 Exploratory Data Analysis (EDA)

## 1️⃣ Market With Most Transactions
Used:
```python
df["Market"].value_counts().head()
```

Purpose:
- Identify markets processing the highest number of transactions.

---

## 2️⃣ Monthly Transaction Trends
Grouped transactions by month to analyze activity trends throughout the year.

Visualization:
- Line plot using Seaborn

Insights:
- Helped identify peak transaction months.

---

## 3️⃣ Top Merchants by Revenue
Grouped merchants by:
```python
df.groupby("Merchant")["Amount_USD"].sum()
```

Purpose:
- Determine merchants generating the highest transaction revenue.

---

## 4️⃣ Market vs Fraud Flag Analysis
Compared:
- Transaction amounts
- Market categories
- Fraud flag status

Visualization:
- Bar plots with `hue="Fraud_Flag"`

Purpose:
- Understand fraud patterns across different markets.

---

## 5️⃣ Payment Type Revenue Analysis
Analyzed:
- Which payment types generate more revenue
- Fraud distribution across payment methods

Visualization:
- Seaborn barplots

---

## 6️⃣ Top Merchants by Fee Revenue
Calculated total `Fee_USD` per merchant.

Visualization:
- Top 10 merchants plotted using bar charts

Purpose:
- Identify merchants contributing most fee revenue.

---

# 📈 Visualizations Created

The project includes:
- Line Charts
- Bar Charts
- Revenue Comparisons
- Fraud Distribution Visualizations

Libraries used:
```python
import matplotlib.pyplot as plt
import seaborn as sns
```


# 📚 Skills Demonstrated

This project demonstrates:
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Data Visualization
- Grouping & Aggregation
- Working with Real-World Transaction Data
- Fraud Analysis

---

## Dashboard
View the live dashboard here:
https://public.tableau.com/authoring/Paywave2024_fraudandrevenueuoverview/Paywave2024frauddetectionandrevenueoverview#1



# 👨‍💻 Author

## Kirema Mutua
Aspiring Data Engineer & Data Analyst



---

# ⭐ Support

If you like this project:
- Star the repository
- Fork the project
- Share feedback
