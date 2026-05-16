# Peakflo — Invoice Sync Intelligence System
### Built by Agila Govindan | agilawork.online

---

## Company Overview
Peakflo is a YC-backed Singapore fintech that helps 
finance teams automate accounts payable and receivable. 
Used by companies across Singapore, India, Indonesia 
and Philippines.

---

## Problem I Identified
When finance teams edit invoices in QuickBooks after 
syncing with Peakflo — Peakflo still shows the old 
amount. Two different numbers appear for the same 
invoice. Finance teams lose trust in the platform 
and go back to manual Excel work. Peakflo loses 
the client.

---

## Solution I Built — 3 Floors + Email Automation

### Floor 1 — Power BI Dashboard
Visual real-time dashboard so finance managers see 
the full picture in 10 seconds every morning.

What it shows:
- Total invoices tracked
- Mismatched invoices count
- Sync health percentage
- Overdue invoices
- High risk client flags
- QuickBooks vs Peakflo amount comparison table
- Top clients by invoice value bar chart
- Filter by payment status and sync status

Tools: Power BI | DAX | Power Query | Excel

---

### Floor 2 — Automated Mismatch Detection (Python)
Python script reads invoice data automatically and 
finds every mismatch between QuickBooks and Peakflo.
Shows exact dollar difference per client and 
specific action required. No manual checking needed.

Tools: Python | Pandas | openpyxl

---

### Floor 3 — Predictive Risk Analysis (Python)
Analyses historical mismatch patterns per client 
and predicts which clients will cause problems next 
time — before the mismatch happens.

Risk levels:
- CRITICAL — 80%+ mismatch rate — set alert immediately
- HIGH RISK — 50-80% — monitor closely  
- STABLE — below 50% — no action needed

Tools: Python | Pandas | GroupBy analysis

---

### Email Automation — Auto Alert to Inbox
When the script runs it sends a fully formatted HTML 
email to the finance team inbox automatically.

Email contains:
- KPI snapshot cards with colour coding
- Full mismatch table with every invoice
- Predictive risk table with badges
- Recommended actions for today, this week, long term

No manual work. No opening Python. No checking 
dashboards. The alert arrives in your inbox and 
tells you exactly what to fix.

Tools: Python | smtplib | HTML email | Gmail SMTP

---

## Full Process Flow# Peakflo_Invoice
