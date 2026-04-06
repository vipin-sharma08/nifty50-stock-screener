# 🔍 NIFTY 50 Stock Screener

> A Python-based screener for filtering NIFTY 50 stocks using technical indicators, pivot levels, and momentum signals.

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python) ![License](https://img.shields.io/badge/license-MIT-green)

---

## ✨ Features

- **RSI Filter** — Screen stocks by overbought/oversold conditions (RSI < 30, > 70)
- **MACD Signal** — Bullish/bearish crossover detection
- **Pivot Levels** — Classic, Camarilla, and Fibonacci pivot support/resistance
- **Volume Spike Detection** — Flag unusual volume relative to 20-day average
- **Export to CSV/Excel** — One-click export of screened results

---

## 📁 Project Structure

```
nifty50-stock-screener/
├── screener.py          # Main screening logic
├── indicators.py        # RSI, MACD, Pivot calculations
├── data_fetch.py        # yfinance data pipeline
├── export.py            # CSV / Excel export
├── config.py            # Tickers list & thresholds
└── requirements.txt
```

---

## 🚀 Quickstart

```bash
git clone https://github.com/vipin-sharma08/nifty50-stock-screener.git
cd nifty50-stock-screener
pip install -r requirements.txt
python screener.py
```

---

## 📊 Sample Output

| Ticker | RSI | MACD Signal | Pivot S1 | Pivot R1 | Volume Spike |
|--------|-----|-------------|----------|----------|--------------|
| RELIANCE | 31.2 | Bullish | 2842.00 | 2910.00 | ✔️ |
| INFY | 68.9 | Bearish | 1480.50 | 1540.00 | ❌ |
| HDFCBANK | 45.1 | Neutral | 1590.00 | 1640.00 | ❌ |

---

## 🛠️ Tech Stack

| Library | Purpose |
|---|---|
| `pandas` | Data manipulation |
| `yfinance` | NSE/BSE market data |
| `TA-Lib` / `pandas-ta` | Technical indicators |
| `openpyxl` | Excel export |

---

## 📝 License

MIT © [Vipin Sharma](https://github.com/vipin-sharma08)
