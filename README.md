# 🧭 Payroll Compass
#### A private, client-side tool for validating Panamanian payroll deductions.

## 😵‍💫 The Problem
Payroll transparency can be a challenge. Employees often struggle to understand why their tax deductions fluctuate throughout the year, especially when variable income (Bonuses, Overtime, XIII Month) is involved.

Standard pay stubs provide a snapshot of a single moment, but they rarely explain the context of how progressive taxes (like ISR) are calculated on a cumulative basis. This leads to confusion, "sticker shock" during bonus months, and unnecessary friction between staff and management.

## 🎯 The Solution
Payroll Compass is a web-based calculator designed to bridge the gap between "What Payroll Deducted" and "What the Law Says."

It allows you to:
- **Digitize your Pay Stubs**: Input your data period-by-period.
- **Validate Deductions**: Instantly compare the taxes deducted against the official Panama 2025 tax tables.
- **Visualize the "Why"**: See cumulative graphs that explain how your effective tax rate changes over time.

## 🔒 Privacy & Data Security
🚨 **This is the most important section. Please read carefully.**

This tool follows a **"Zero-Knowledge"** architecture.

- **Client-Side Only**: All calculations happen 100% inside your web browser (Chrome, Edge, Safari).
- **No Database**: There is no backend server. We do not store your salary, your name, or your financial data.
- **No Transmission**: When you click "Add Pay Stub," data moves from your keyboard to your browser's temporary memory (RAM). It is NEVER sent over the internet.
  - The same is true when you "Import" your CSV backup file, the data moves from your CSV file to your browswer's temporary memory (RAM) and NEVER sent over the internet.
- **Session-Based**: If you refresh the page, your data is gone forever—unless you explicitly choose to export a backup.

### How to Verify
You can disconnect your internet after loading the page. The tool will continue to function perfectly, proving that it does not need to "phone home" to work.

## 🧑‍🏫 How to Use
### A. The Editor (Left Panel)
1. **Date**: Select the date of your pay stub.
2. **Income**: Enter your Base Salary.
  - Use the toggle buttons **[QBP]**, **[OT]**, **[VAC]** to reveal inputs for variable income.
  - **[XIII]**: This toggle only appears if the selected date is within a valid payment window (Apr 1-15, Aug 1-15, Dec 1-15).
  - **Totals**: The editor updates "GROSS SALARY" (Taxable Base) and "TOTAL EARNINGS" (Base + GREP + Home) in real-time.
3. **Taxes**: Enter the actual tax amounts shown on your physical pay stub (SS, SE, ISR).
4. **Deductions**:
  - Insurance: Use this entry to document additional Insurance deductions (what you pay for spouse or children beneficiaries)
  - **Loans**: Use the toggle buttons (L1 - L5) to manage up to 5 distinct loan slots.
5 Actions:
  - **Add Pay Stub**: Commits the data to the ledger.
  - **Edit**: Clicking the ✏️ pencil icon on a row pulls data back to the editor for safe modification without deleting the original until you save.

### B. Interpreting the Data
**The Dashboard (KPIs)**
1. **YTD Cash Flow**: A waterfall view showing your Total Income minus Taxes and Deductions, resulting in your Net Pay.
2. **XIII Estimator**: A smart projection of your next 13th Month payment.
  - Config: Click the ⚙️ gear icon to enter "Carryover" income from Dec 16-31 of the previous year for accurate April projections.
3. **YTD Deductions**: Breaks down Insurance and individual Loans. 
4. **ISR Cards**:
  - Comparing **Paid** (Payroll) vs. **Legal** (Calculator).
  - **Legal**: What the strict annual tax table says you owe.
  - **Micro-Charts**: The visual curve shows the gap between Paid (Red) and Legal (Green) accumulation.

**The Ledger (Table)**
1. **Granularity**: Every income type (OT, Vac, etc.) gets its own column if used.
2. **Effective Rates**: Below every tax dollar amount, you will see the Effective %. This helps identify exactly which rate was applied to that specific check.
3. **YTD Section**: The right side of the table shows running totals for the year.

### C. Saving Your Data
Since we don't store your data, you must manage it yourself:
- At the top right corner, click the **[Export]** button to save a file to your computer.
- Next time you visit, click the **[Import]** button and select that file to pick up where you left off.

## Disclaimer
This tool is for educational and validation purposes only. It is built based on the Panamanian Tax Code (Código Fiscal) as of 2025. While it strives for 100% accuracy, official payroll calculations may vary due to specific internal accounting practices. Always consult with HR for official disputes.
