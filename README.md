# Sector Resilience During the COVID-19 Market Crash

## Overview

This project analyzes how different U.S. equity market sectors responded to the COVID-19 market shock in early 2020.  
Sector resilience is evaluated using three quantitative metrics:

- Maximum drawdown during the crash
- Speed of recovery to pre-crash levels
- Total return during the remainder of 2020

The goal is to compare how defensive and cyclical sectors behaved during a major economic shock using transparent, reproducible analysis.

---

## Data Source

- Daily adjusted closing prices for U.S. sector ETFs
- Data retrieved using the `yfinance` Python library
- Sector ETFs are used as proxies for S&P 500 sector performance

---

## Methodology

The COVID-19 market crash is defined as:

- **Peak:** February 19, 2020  
- **Bottom:** March 23, 2020  

For each sector, the following metrics are computed:

1. **Maximum Drawdown**  
   Largest peak-to-trough decline during the crash window.

2. **Recovery Speed**  
   Number of calendar days required to recover to the pre-crash peak level after March 23, 2020.

3. **Post-Crash Total Return**  
   Cumulative return from February 19, 2020 through December 31, 2020.

Each sector is ranked across these dimensions and combined into an equal-weight overall resilience score.

---

## Key Results

- Technology (XLK) and Consumer Discretionary (XLY) showed the fastest recovery and strongest post-crash returns.
- Energy (XLE) experienced the deepest drawdown and slowest recovery.
- Defensive sectors generally limited drawdowns but lagged in post-crash upside.

These results highlight meaningful differences between cyclical and defensive sectors during the COVID-19 shock.

---

## Repository Structure

```text
├─ sector_resilience_covid.ipynb   # Full analysis notebook
├─ sector_resilience_results.csv   # Final ranked results table
├─ Sector Resilience COVID19 Data Analysis.pptx   # Presentation summarizing analysis and results
├─ README.md
├─ LICENSE

```

---

## Tools & Skills Demonstrated

- Python (pandas, numpy, matplotlib)
- Financial return and drawdown analysis
- Time-series data handling
- Quantitative comparison of market sectors
- Clear analytical storytelling for economic events

---

## Motivation

This project was developed as a portfolio piece to demonstrate applied data analytics and financial reasoning in the context of real-world market stress events. It emphasizes transparency, interpretability, and economic intuition rather than black-box modeling.
