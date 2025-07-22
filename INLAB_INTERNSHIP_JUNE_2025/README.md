# 🛒 Dynamic Price Prediction System

This project presents a hybrid **dynamic pricing engine** for Amazon sellers. The system generates optimal, competitive, and profit-aware product prices based on market trends, competitor data, and business constraints.

---

## 📈 Features

- **Real-Time Scraping:** Uses BeautifulSoup to extract Amazon competitor prices, ratings, and reviews.
- **Demand Forecasting:** Uses ARIMA on Google Trends data to estimate product popularity.
- **ML Prediction:** XGBoost regressor trained on rating, review count, sales, and trend score.
- **Heuristic Rules:** Adjust prices based on stock, product age, and demand score.
- **Web Interface:** Flask UI for entering inputs and displaying predictions with CSV export.

---

## 🧪 Technologies Used

- Python, Flask
- BeautifulSoup, PyTrends
- ARIMA (Statsmodels)
- XGBoost
- Pandas, NumPy, Matplotlib

---

## 🗃️ Data Sources

- **Amazon Product Pages**: Real-time scraped listings.
- **Google Trends**: 90-day product search interest time series.
- **Manual Inputs**: Cost, stock, product age.

---

## 📊 Evaluation Metrics

| Model | RMSE | MAE | MAPE |
|-------|------|-----|------|
| ARIMA + XGBoost | ₹348.20 | ₹325.07 | 22.14% |
| Prophet + LightGBM | ₹590.74 | ₹584.67 | 57.32% |
| Bayesian Ridge | ₹487.12 | ₹344.80 | 38.73% |

---

## 📦 Output

- Base and Final Price with Adjustment Breakdown
- Competitor Listings
- Google Trends + ARIMA Forecast Graph
- Downloadable CSV report

---

## 🧠 Future Enhancements

- Switch to LSTM/Transformer for seasonality
- Integrate Flipkart/Snapdeal scraping
- Add calendar-aware pricing (festival days)
- Deploy dashboard + user accounts + API integration
