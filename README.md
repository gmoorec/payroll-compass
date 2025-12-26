# 🧭 Payroll Compass
#### A private, client-side tool for validating Panamanian payroll deductions.

## 😵‍💫 The Problem
Payroll transparency can be a challenge. Employees often struggle to understand why their tax deductions fluctuate throughout the year, especially when variable income (Bonuses, Overtime, XIII Month) is involved.

Standard pay stubs provide a snapshot of a single moment, but they rarely explain the context of how progressive taxes (like ISR) are calculated on a cumulative basis. This leads to confusion, "sticker shock" during bonus months, and unnecessary friction between staff and management.

## 🎯 The Solution
Payroll Compass is a web-based calculator designed to bridge the gap between "What Payroll Deducted" and "What the Law Says."

It allows you to:

- Digitize your Pay Stubs: Input your data period-by-period.
- Validate Deductions: Instantly compare the taxes deducted against the official Panama 2025 tax tables.
- Visualize the "Why": See cumulative graphs that explain how your effective tax rate changes over time.
- Forecast: Understand how a future bonus might impact your net pay.

## 🔒 Privacy & Data Security
🚨 **This is the most important section. Please read carefully.**

This tool follows a **"Zero-Knowledge"** architecture.

- Client-Side Only: All calculations happen 100% inside your web browser (Chrome, Edge, Safari).
- No Database: There is no backend server. We do not store your salary, your name, or your financial data.
- No Transmission: When you click "Add Pay Stub," data moves from your keyboard to your browser's temporary memory (RAM). It is never sent over the internet.
- Session-Based: If you refresh the page, your data is gone forever—unless you explicitly choose to export a backup.

### How to Verify
You can disconnect your internet after loading the page. The tool will continue to function perfectly, proving that it does not need to "phone home" to work.

## 🧑‍🏫 How to Use
#### A. Getting Started
- Open the tool in your browser.
- Select the **Date** of your pay stub.
- **Income**: Enter your Base Salary. Use the toggle buttons (QBP, OT, VAC) to add other income types found on your stub.
  - Note: The "XIII Mes" button will only appear if the date is within a valid payment window (April, August, December).
- **Taxes**: Enter the actual tax amounts shown on your physical pay stub (SS, SE, ISR).
- **Deductions**: Add loans or insurance if applicable.
- Click **Add Pay Stub**.

#### B. Interpreting the Data
**The Dashboard (KPIs)**
- **YTD Cash Flow**: A waterfall view showing your Total Income minus Taxes and Deductions, resulting in your Net Pay.
- **ISR Comparisons**:
  - **Paid**: What the company took out.
  - **Legal**: What the strict annual tax table says you owe.
  - The Graph: If the **Red Line** (Paid) is above the **Green Line** (Legal), you are currently "ahead" on taxes and might see lower deductions later in the year.

**The Ledger (Table)**
- **Columns**: Each column represents a specific component (Base, Overtime, SS, ISR).
- **Percentages**: Below every tax dollar amount, you will see the Effective Rate (e.g., 9.75%). This helps you catch errors where the wrong rate was applied.
- **YTD Section**: The right side of the table shows running totals for the year.

#### C. Saving Your Data
Since we don't store your data, you must manage it yourself:
- Click Export CSV to save a .csv file to your computer.
- Next time you visit, click Import and select that file to pick up where you left off.

## Disclaimer
This tool is for educational and validation purposes only. It is built based on the Panamanian Tax Code (Código Fiscal) as of 2025. While it strives for 100% accuracy, official payroll calculations may vary due to specific internal accounting practices. Always consult with HR for official disputes.
