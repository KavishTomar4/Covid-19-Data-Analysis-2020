# 🦠 Covid-19 Data Analysis 2020

Exploratory data analysis of global Covid-19 trends in 2020 using Python and Pandas — tracking confirmed cases, deaths, recoveries, and the progression of the pandemic over time.

---

## 📌 Project Overview

This project analyses the [Covid-19 Dataset](https://www.kaggle.com/datasets/imdevskp/corona-virus-report) from Kaggle containing day-wise global Covid-19 statistics throughout 2020. The goal was to understand how the pandemic spread and evolved over time using data analysis and visualization.

---

## 🛠️ Tech Stack

- **Python** — Pandas, NumPy, Matplotlib
- **Jupyter Notebook** — Analysis environment

---

## 📂 Dataset

**File:** `day_wise.csv`

| Column | Description |
|---|---|
| `Date` | Date of record |
| `Confirmed` | Total confirmed cases |
| `Deaths` | Total deaths |
| `Recovered` | Total recovered cases |
| `Active` | Currently active cases |
| `New cases` | New cases reported that day |
| `New deaths` | New deaths reported that day |
| `New recovered` | New recoveries reported that day |
| `Deaths / 100 Cases` | Death rate per 100 cases |
| `Recovered / 100 Cases` | Recovery rate per 100 cases |

---

## 🔍 Key Analyses

### 1. 📈 Global Cases Trend Over Time
- Tracked daily confirmed, deaths and recovered cases from Jan–Dec 2020
- Visualized the exponential growth of the pandemic

**Finding:** Confirmed cases grew exponentially from March 2020 onwards, with the steepest rise seen between June and December 2020.

---

### 2. 💀 Daily New Cases vs New Deaths
- Compared new cases and new deaths reported each day
- Identified peak waves of the pandemic in 2020

**Finding:** The first major wave peaked around April 2020, followed by a much larger second wave from October 2020 onwards.

---

### 3. 📊 Death Rate vs Recovery Rate Over Time
- Calculated death rate = Deaths / Confirmed Cases × 100
- Tracked how mortality rate changed as the pandemic progressed

**Finding:** Death rate was highest (~7%) in early April 2020 when healthcare systems were overwhelmed, gradually declining to ~2.5% by December 2020 as treatments improved.

---

### 4. 🔢 Active Cases Trend
- Tracked active cases (Confirmed - Deaths - Recovered) over time
- Shows the true burden on healthcare systems at any point

**Finding:** Active cases peaked dramatically in late 2020, indicating the pandemic was far from under control by year end.

---

## 🧹 Data Cleaning

| Issue | Fix |
|---|---|
| Date column stored as string | Converted to datetime |
| Missing values in rate columns | Filled with 0 |
| Inconsistent date formatting | Standardized with `pd.to_datetime()` |

---

## 📊 Key Findings

| Metric | Value |
|---|---|
| Peak daily new cases (2020) | ~700,000+ cases/day |
| Highest death rate | ~7% in April 2020 |
| Death rate by Dec 2020 | ~2.5% |
| Total confirmed by end 2020 | 83M+ cases globally |

---

## 🚀 How to Run

1. Clone the repository
```bash
git clone https://github.com/KavishTomar4/Covid-19-Data-Analysis-2020.git
cd Covid-19-Data-Analysis-2020
```

2. Install dependencies
```bash
pip install pandas numpy matplotlib
```

3. Run the notebook
```bash
jupyter notebook covid_19.ipynb
```

---

## 📁 Project Structure

```
Covid-19-Data-Analysis-2020/
│
├── covid_19.ipynb       # Main analysis notebook
├── day_wise.csv         # Dataset
└── README.md            # Project documentation
```

---

## 💡 Conclusion

> The Covid-19 pandemic showed explosive exponential growth through 2020. Death rates were highest in early April when healthcare systems were unprepared, but gradually improved as treatments advanced. The second wave in late 2020 was significantly larger than the first, highlighting the failure of early containment efforts globally.

---

## 👤 Author

**Kavish Tomar**
[GitHub](https://github.com/KavishTomar4)
