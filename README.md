# automated-finance-dashboard-excel
Automated finance dashboard in Excel powered by Power Automate. Real-time transaction tracking directly from emails with automated category &amp; summary reports.


This project is a fully automated personal finance tracking system.  
It combines **Excel**, **Power Automate**, and **financial logic** to create a dynamic dashboard that updates itself every time a new transaction email arrives.

## What this project demonstrates

### 1. Excel Skills
- Structured tables
- Dynamic dashboards
- Category-based analysis
- Monthly deviation calculations
- Lookup formulas and conditional logic

### 2. Power Automate Skills
- Email triggers (Outlook)
- Parsing HTML bodies
- Extracting amounts without regex
- Conditional logic for account classification
- Writing rows into Excel tables automatically

### 3. Finance Knowledge
- Separation of debit vs credit accounts
- Categorization of expenses and income
- Monthly performance tracking
- Savings rate calculation
- Merchant-based analysis

## How the system works

1. **Outlook receives a transaction email**  
   (CIBC, SCOTIABANK, Interac, ATM, Costco Mastercard, etc.)

2. **Power Automate extracts key fields**  
   - Date  
   - Amount  
   - Account (DC CIBC or CC CIBC or CC SCOTIA)  
   - Details (merchant or transfer info)

3. **Power Automate writes the row into Excel**  
   The table `tTransactions` is the single source of truth.

4. **Excel dashboard updates automatically**  
   Charts, totals, averages, deviations, and savings rate refresh instantly.

See `/docs/architecture.md` for a full breakdown.

