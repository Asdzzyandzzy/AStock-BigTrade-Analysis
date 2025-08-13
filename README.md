# 📊 A-Share Tick Trade Analyzer (Large Orders) by zzy

A Streamlit-based web application for **real-time analysis** of A-share tick-level trade data.  
It uses the [`akshare`](https://github.com/akfamily/akshare) API to fetch **tick-by-tick transactions** and provides powerful filtering, aggregation, and visualization functions, especially for large trades.

---

## ✨ Features

- **Real-time tick data** retrieval via `akshare`  
- **Custom trade amount filtering** (min / max range)  
- **Amount range banding** with flexible bins (0-15万, 15-50万, 50-200万, 200万+)  
- **Nature-based statistics** (Buy, Sell, Neutral)  
- **Weighted average price** calculation  
- **Total row in pivot tables** for quick summary  
- **Horizontal bar charts**: Price vs. Total Trade Amount, split into 5 categories  
- **Data export** to CSV for both raw trades and summary tables  
- **Optional raw data view** for detailed inspection

---

## 📸 Screenshots

### 1. Main Interface
<img width="1920" height="1139" alt="image" src="https://github.com/user-attachments/assets/5c42ed91-d441-4384-89d9-88f7efc9ebd5" />


### 2. Amount Range Filtering
<img width="1488" height="665" alt="image" src="https://github.com/user-attachments/assets/79d5f4ba-6c96-41ea-8a7a-c32b1101a191" />

### 3. Horizontal Price Distribution Charts
<img width="1526" height="674" alt="image" src="https://github.com/user-attachments/assets/77ee4bda-6f85-4b03-872a-28902a0f1ef8" />
<img width="1514" height="760" alt="image" src="https://github.com/user-attachments/assets/1da8419d-2165-4cd6-880b-dab59b237937" />
<img width="1420" height="650" alt="image" src="https://github.com/user-attachments/assets/2b968f9e-3487-4d0a-a311-e485295e7abb" />
<img width="1484" height="649" alt="image" src="https://github.com/user-attachments/assets/40c84b35-1625-4765-a197-4b9d308b6db2" />


---

## 🛠 Installation

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/ashare-tick-analyzer.git
cd ashare-tick-analyzer
```

### 2. Create a virtual environment (recommended)
```bash
python -m venv venv
source venv/bin/activate   # On macOS/Linux
venv\Scripts\activate      # On Windows
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

---

## 📦 Requirements

- Python 3.8+
- [Streamlit](https://streamlit.io/)
- [Pandas](https://pandas.pydata.org/)
- [NumPy](https://numpy.org/)
- [AkShare](https://github.com/akfamily/akshare)
- [Plotly](https://plotly.com/python/) (for interactive charts)

---

## 🚀 Usage

Run the app locally:

```bash
streamlit run app.py
```

### Parameters (in Sidebar)

- **Stock Code**: Full code with exchange prefix (e.g., `sh600941`, `sz000001`)
- **Amount Range**: Min and max trade amount in CNY
- **Show Raw Data**: Optional checkbox to view the entire tick dataset

---

## 📊 Analysis Output

1. **KPI Cards**: Total trades, total amount, amount range  
2. **Nature-based Summary**: Amount sum & weighted average price  
3. **Detailed Trades Table**: All trades within selected amount range  
4. **Banding Summary**: Number of trades, total amount, weighted average price per range  
5. **Pivot Table (Band × Nature)**: Includes row/column totals  
6. **Horizontal Price Distribution Charts**:  
   - **Total** (all trades)  
   - **Four amount bands** individually  
   - Y-axis = price, X-axis = total trade amount, horizontal bars for better trend view

---
