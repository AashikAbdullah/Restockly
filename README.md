
# 📦 Restockly – AI-Powered Restock Advisor for Small Businesses

**Restockly** is a lightweight, intelligent inventory restocking assistant built with machine learning. It empowers small-scale and individual sellers to accurately forecast short-term demand and plan restocking with confidence, using only sales data and minimal setup.

---

## ✅ Key Features

- 🔮 **7-Day Demand Forecasting** using Linear Regression  
- 📅 **Time Series Alignment** by filling in missing sales dates with zero  
- 📦 **Product-Level Forecasting** for personalized restock plans  
- 📁 **CSV Export** of final restocking recommendations  
- 🧠 **Jupyter Notebook Implementation** for full transparency and flexibility

---

## 🧪 Repository Contents

| File                          | Description                                                  |
|-------------------------------|--------------------------------------------------------------|
| `restockly_validation.ipynb`  | Main notebook: data cleaning, EDA, forecasting, restock calc |
| `sample_sales_data.csv`       | Sample input dataset for testing and demonstration           |
| `README.md`                   | Project documentation (this file)                            |

---

## 🛠️ How to Use

### 1. Clone the repository:
```bash
git clone https://github.com/AashikAbdullah/Restockly.git
cd Restockly
```

### 2. Install dependencies:
```bash
pip install pandas scikit-learn matplotlib seaborn
```

### 3. Launch the notebook:
```bash
jupyter notebook restockly_validation.ipynb
```

### 4. Prepare your sales data:
A CSV file with the following structure is required:

| Product     | Date       | Quantity Sold |
|-------------|------------|----------------|
| Product_1   | 2024-05-01 | 10             |

> You can optionally include a `Current Stock` column to receive detailed restock suggestions.

---

## 📈 Forecasting Logic

Restockly uses Linear Regression to forecast product demand for the next 7 days. It calculates how much stock you should reorder based on the forecast and current stock levels.

```
Restock Quantity = Forecasted Demand - Current Stock + Buffer
```

---

## ✅ Sample Output

| Product     | Forecasted Demand | Current Stock | Recommended Restock |
|-------------|--------------------|----------------|----------------------|
| Product_10  | 52                 | 20             | 37                   |

---

## 👨‍💻 Author

**Aashik Abdullah**  
Student Project – Inventory Forecasting Tool  
GitHub: https://github.com/AashikAbdullah

