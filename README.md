Customer Transactions Portfolio Analysis (R) 

📌 Project Overview

This project analyzes a customer transaction portfolio using R. 
The goal is to explore customer activity, financial performance, refunds behavior, and card scheme distribution based on Last Twelve Months (LTM) metrics. 

The analysis focuses on:
Transaction volumes and amounts
Customer activity segmentation (online vs physical POS)
Financial performance (MSC, NET MSC)
Refund behavior
Card scheme distribution and comparison
This project is suitable for a Data Analyst portfolio, demonstrating data cleaning, descriptive statistics, and data visualization in R. 

Key Columns Used

TRX_COUNT_LTM – Number of transactions (LTM)
TRX_AMOUNT_LTM – Total transaction amount (LTM)
ONLINEPOS – Transaction channel (ONLINE or POS)
MSC_LTM – Gross merchant service charge (profit)
NET_MSC_LTM – Net profit
REFUND_AMOUNT_LTM – Refund amount
SCHEME – Card scheme (e.g. VISA, Mastercard) 

Removed Columns (Data Validation Step)

CB_COUNT
CB_AMOUNT
FRAUD_COUNT
FRAUD_AMOUNT
These columns were excluded to keep the analysis focused on transaction and revenue behavior. 

🛠️ Technologies Used
R
Base R (statistics, subsetting)
ggplot2 (visualization) 

🔎 Analysis Steps
1️⃣ Data Loading & Validation
Imported CSV data using read.csv()
Removed chargeback and fraud-related columns
Performed initial inspection using head() 

2️⃣ Customer Activity Analysis
Transaction Volume
Calculated mean and median of transaction amounts
Visualized distribution using a histogram
Activity Segmentation
Segmented customers into:
Online transactions
Physical POS transactions
Visualization
Scatter plot of:
TRX_COUNT_LTM vs TRX_AMOUNT_LTM
This helps identify high-frequency and high-value customers. 

3️⃣ Financial Performance Analysis
Metrics Calculated
Mean and median of MSC_LTM
Total net profit (NET_MSC_LTM)
Standard deviation of gross profit
Visualization
Histogram of MSC_LTM to understand profit distribution 

4️⃣ Refund Analysis
Metrics Calculated
Mean refund amount
Total refund volume
Visualization  
Histogram of refund amounts to identify refund patterns and outliers 


5️⃣ Card Scheme Analysis
Card Type Distribution
Count of transactions by card scheme
Percentage share per card type
Visualizations
Bar chart: number of transactions by card scheme
Pie chart: percentage share of each scheme
Comparative Analysis
Boxplot comparing TRX_AMOUNT_LTM across card schemes
This highlights differences in transaction behavior between card networks. 

📊 Key Insights (Example)
Transaction amounts are right-skewed, indicating a small number of high-value customers
Online and POS transactions show different volume patterns
Certain card schemes are associated with higher median transaction values
Refund amounts are concentrated around low values, with some outliers  

📈 Future Improvements
Add customer segmentation (low / medium / high value)
Time-based analysis if date-level data becomes available
Correlation analysis between refunds and transaction volume
Dashboard version using Shiny or Power BI



