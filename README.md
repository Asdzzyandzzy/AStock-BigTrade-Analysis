# AStock-BigTrade-Analysis

A Streamlit-based data analysis tool for filtering and visualizing large transactions in China's A-share market using [AKShare](https://akshare.xyz/).

## 📌 Features
- Fetch tick-by-tick trade data for a given A-share stock.
- Filter transactions larger than a specified amount.
- Group by trade type (buy, sell, neutral) to calculate:
  - Total traded amount
  - Weighted average price (amount-weighted)
- Interactive UI with customizable parameters.
- Export large trade details and summary as CSV files.
- Optional display of raw tick data.

---

## 📦 Installation

1. **Clone the repository**
```bash
git clone https://github.com/<your-username>/AStock-BigTrade-Analysis.git
cd AStock-BigTrade-Analysis





## Usage
```bash
streamlit run app.py
