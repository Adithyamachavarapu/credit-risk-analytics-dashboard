# credit-risk-analytics-dashboard
A credit risk analysis project built in Excel. It takes a loan dataset of 32,000+ records and turns it into a clean dashboard showing default rates, money at risk, and risk by income and credit grade — plus an insights page with recommendations. Built fully with native Excel formulas and charts.

# Credit Risk Analytics Dashboard 📊

An interactive **Excel dashboard** that analyses a portfolio of 32,500+ loans to show
who is likely to default, how much money is at risk, and what the business should do
about it — all built with native Excel formulas and charts.

---

## 📸 Preview

<img width="890" height="612" alt="Screenshot 2026-06-15 at 14 00 09" src="https://github.com/user-attachments/assets/692276fe-a810-4832-9860-f265be362ea6" />
<img width="781" height="615" alt="Screenshot 2026-06-15 at 14 00 40" src="https://github.com/user-attachments/assets/c30205e4-a9ac-4269-91a7-3ce57386d6d5" />

---

## 🧐 What this project does

It takes a raw loan dataset and turns it into a clean, easy-to-read dashboard that
answers three simple questions:

1. **How risky is our loan book?**
2. **Which loans go bad, and why?**
3. **What should we do about it?**

Everything is live — change the data and the numbers, charts, and KPIs update by themselves.

---

## 📂 Inside the file (4 sheets)

The workbook is split into four pages, each with a clear job:

### 1. `credit_risk_dataset` — the Data page
This is the raw data — the original CSV of every loan (age, income, loan amount,
grade, whether it defaulted, etc.). Think of it as the "source of truth." Two helper
columns were added to clean out a few bad records and to group loans by risk band.

### 2. `cal` — the Calculation page
This is the "engine room." It holds the summary tables (pivots) that feed the dashboard —
total loans, default rate, money at risk, default rates by income band, by grade, and the
loan status split. Nothing fancy to look at; it just does the maths so the dashboard stays accurate.

### 3. `dasboard` — the Dashboard page
The main visual. A dark, modern dashboard with:
- **5 KPI cards** — Total Loans, Default Loans, Risk Exposure, Avg Default Loan, Avg Loan
- **Default Rate by Loan-to-Income** (bar chart)
- **Loan Status Split** (donut chart)
- **Default Rate by Grade** (line chart)

This is the page you'd show in a meeting.

### 4. `insights` — the Insights page
The "so what." Plain-English findings and recommendations — written for anyone, not just
analysts. Each insight comes with a simple fix (e.g. *"Don't lend more than 30% of a person's income"*).

---

## 🔑 Key findings

- **1 in 5 loans default (≈22%)** — about ₹7.7 crore at risk. That's high.
- **Loan-to-income is the biggest warning sign** — under 30% of income is mostly safe;
  above 30%, more than half of loans default.
- **Low grades rarely pay back** — Grades A–C are healthy (10–21%), but Grade G defaults **98%** of the time.
- **Bigger loans are riskier** — defaulted loans are larger on average than normal loans.
- **78% of borrowers pay back fine** — the safe core of the book is solid.

**Bottom line:** Most losses come from a few clear cases — *big loans + low grades*.
Controlling those two cuts bad loans sharply while keeping most of the good business.

---

## 🛠️ Built with

- **Microsoft Excel** — formulas (`COUNTIFS`, `SUMIFS`, `AVERAGEIFS`), native charts, conditional design
- No add-ins or macros — opens and works in any modern Excel

---

## 🚀 How to use

1. Download `credit_risk_dashboard.xlsx`
2. Open it in Excel
3. Go to the **dasboard** tab to explore the visuals, or **insights** for the recommendations
4. To use your own data, paste it into the **credit_risk_dataset** sheet — everything updates automatically

---

## 📁 Files

```
credit_risk_dashboard.xlsx   # the full workbook (data + cal + dashboard + insights)
credit_risk_dataset.csv      # the raw source data
```

---

*Built as a credit-risk analytics project to practice data cleaning, KPI design, and dashboard storytelling in Excel.*
