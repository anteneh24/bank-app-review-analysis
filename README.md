# 📊 Week 2 - Task 1: Data Collection and Preprocessing

This repository contains the code and data for **Task 1** of the Week 2 challenge at Omega Consultancy: analyzing customer satisfaction for mobile banking apps in Ethiopia.

---

## 🧾 Objective

To **scrape**, **clean**, and **prepare** Google Play Store reviews for three major Ethiopian banks:

- **Commercial Bank of Ethiopia (CBE)**
- **Bank of Abyssinia (BOA)**
- **Dashen Bank**

---

## 🔍 Methodology

### 1. 🔗 Scraping Reviews

- Used the [`google-play-scraper`](https://pypi.org/project/google-play-scraper/) Python package.
- Collected the following fields:
  - **Review Text**
  - **Rating (1–5)**
  - **Review Date**
  - **App/Bank Name**
  - **Source** (always "Google Play")
- Targeted **400+ reviews per bank**, totaling over **1,200 reviews**.
- Scraping was performed in: `Notebook/scraper.ipynb`

---

### 2. 🧹 Preprocessing

- Removed **duplicate reviews** based on review text and date.
- Dropped entries with **missing review text** or **rating**.
- Normalized dates to **`YYYY-MM-DD`** format.
- Standardized column names:
  - `review`
  - `rating`
  - `date`
  - `bank`
  - `source`
- Preprocessing was done in: `Notebook/cleaning.ipynb`

---

## ✅ KPI Checklist

| KPI                      | Status |
| ------------------------ | ------ |
| 1,200+ reviews collected | ✅     |
| <5% missing data         | ✅     |
| Cleaned CSV dataset      | ✅     |
| Organized GitHub repo    | ✅     |
| README with methodology  | ✅     |
