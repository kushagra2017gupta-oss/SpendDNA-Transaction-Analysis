
# SpendDNA: Rahul Sharma Transaction Analysis

## Project Overview
This project analyses Rahul Sharma’s 6-month bank transaction history and builds a behavioural spending profile ("SpendDNA") using **Python, Pandas, and NumPy**.

The aim of the project is not just to calculate totals, but to uncover meaningful financial behaviour patterns such as:
- where money is being spent,
- which vendors dominate spending,
- how spending changes over time,
- what time of day spending usually happens,
- which transactions are unusual,
- and what kind of spender Rahul appears to be overall.

The project combines data cleaning, transaction categorisation, vendor extraction, anomaly detection, behavioural pattern analysis, and final financial reporting in a single notebook-based workflow.

---

## Dataset
- **File used:** `rahul_transactions.csv`
- **Time period covered:** January 2024 to June 2024
- **Total transactions analysed:** 1,310

---

## Objectives
The main objectives of this project were to:

1. Clean and standardise raw bank transaction data  
2. Extract vendor / merchant names from messy transaction descriptions  
3. Categorise transactions into meaningful spending buckets  
4. Generate an executive spending overview  
5. Analyse monthly spending trends across categories  
6. Study time-of-day and day-of-week spending behaviour  
7. Detect unusually large or anomalous transactions  
8. Build spending archetypes based on transaction behaviour  
9. Generate a final text-based SpendDNA financial report

---

## Features Implemented

### 1. Data Cleaning
- Standardised column names
- Cleaned and converted amount values into numeric format
- Parsed and standardised dates
- Checked missing values and duplicate records

### 2. Vendor Extraction
Raw transaction descriptions were processed to identify and clean vendor names.  
Examples include:
- Amazon
- Swiggy
- Uber
- Ola
- Blinkit
- Zepto
- Zerodha
- Rent
- P2P Transfer

### 3. Category Mapping
Transactions were grouped into meaningful spending categories such as:
- E-commerce
- Food Delivery
- Investments
- Personal Transfer
- Rent
- Quick Commerce
- Transport
- Cafe
- Groceries
- Entertainment
- Utilities
- Restaurants
- Others

### 4. Spending Overview
Generated headline financial metrics including:
- Total credits
- Total debits
- Net savings / overspending
- Savings rate
- Total transaction count
- Top categories by spend
- Top vendors by spend

### 5. Monthly Trend Analysis
Built a category × month spending matrix to analyse how Rahul’s spending changed from **January to June 2024**.  
Also identified categories showing the biggest growth and decline over time.

### 6. Time-of-Day & Day-of-Week Analysis
Analysed Rahul’s spending behaviour based on:
- **hour of the day**
- **day of the week**
- peak category hours
- weekday vs weekend spending differences

This helped surface behavioural insights such as late-night food ordering and convenience-driven spending patterns.

### 7. Anomaly Detection
Used **category-wise z-score analysis** to identify unusually large transactions compared to Rahul’s normal spending behaviour within each category.

The anomaly report highlights transactions that significantly deviate from category averages.

### 8. Spending Archetypes
Based on transaction behaviour, Rahul was assigned to multiple spending archetypes such as:
- **The Foodie**
- **The Investor**
- **The Late-Night Snacker**
- **The Shopaholic**
- **The Big Spender**

A custom archetype was also designed for this project:

### **The Convenience Maximalist**
This archetype captures users whose spending is heavily concentrated in:
- Food Delivery
- Quick Commerce
- Cafe spending

Rahul matched this archetype based on the combined share of these convenience-driven categories in his total debit spend.

### 9. Final SpendDNA Report
A final text-based financial report was generated that consolidates:
- executive summary
- top categories
- top vendors
- time-of-day insights
- monthly trend summary
- anomalies
- spending archetypes
- final behavioural verdict

---

## Key Insights from the Analysis

Some major findings from Rahul’s transaction data:

- Rahul is an **over-spender overall**, with total debits significantly higher than total credits.
- **E-commerce** is the highest spending category.
- **Amazon** is the top spending vendor.
- Rahul shows a noticeable **late-night food delivery pattern**, indicating convenience-led spending behaviour.
- A meaningful portion of his money is also allocated to **investments**, showing that his spending behaviour is a mix of impulsive and planned financial decisions.
- The custom archetype **Convenience Maximalist** further highlights Rahul’s strong dependence on convenience spending channels.

---

## Tech Stack
- **Python**
- **Pandas**
- **NumPy**
- **Jupyter Notebook / Google Colab**

---

## Learning Outcomes
This project helped strengthen practical skills in:
- data cleaning and preprocessing
- string parsing for financial transaction descriptions
- vendor standardisation and mapping
- category engineering
- groupby and pivot-table based analysis
- behavioural analytics using transaction data
- anomaly detection using z-score
- financial storytelling through text-based reporting

---

## Project Structure
```bash
SpendDNA-Transaction-Analysis/
│
├── SpendDNA_Rahul_Transaction_Analysis.ipynb
├── DATA SET FOR DADS JUNE.csv      
└── README.md
