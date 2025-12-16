# 📦 Inventory Forecasting & Supply Chain Optimization

## 📌 Overview
This project implements an end-to-end **inventory forecasting and supply chain analytics** solution to help organizations anticipate demand, identify stock-out risks, and support data-driven inventory planning.

The application processes historical inventory and sales data, applies analytics-based forecasting logic, and exposes results through a lightweight web dashboard deployed on **Vercel**.

---

## 🎯 Problem Statement
Supply-chain teams often face challenges such as:
- Stock-outs caused by inaccurate demand estimation  
- Excess inventory leading to higher holding costs  
- Limited visibility into inventory health and risk  

This project addresses these challenges by combining **Python-based analytics** with a **simple, deployable web interface**.

---

## 🧱 Architecture
Inventory CSV Data
↓
Python Analytics (Pandas)
↓
Forecast & Risk Calculation
↓
FastAPI REST API
↓
HTML + JavaScript UI
↓
Vercel Deployment


---

## 🛠️ Technology Stack
- **Python** – Data processing and forecasting logic  
- **Pandas / NumPy** – Data analysis  
- **FastAPI** – Backend REST service  
- **HTML / JavaScript** – Frontend UI  
- **Vercel** – Cloud deployment  

---

## 📂 Project Structure
inventory-forecasting/
│
├── data/
│ └── inventory_sales.csv
│
├── backend/
│ ├── main.py
│ ├── forecasting.py
│ └── requirements.txt
│
├── frontend/
│ └── index.html
│
├── vercel.json
└── README.md


---

## 📊 Dataset
The dataset contains historical inventory and sales data.

**Columns**
- `product_id` – Product identifier  
- `date` – Date of transaction  
- `units_sold` – Units sold per day  
- `stock_level` – Available inventory  

Sample data:
```csv
product_id,date,units_sold,stock_level
P1001,2024-01-01,120,500
P1001,2024-01-02,135,380
P1002,2024-01-01,80,420

---


## ⚙️ **Forecasting Logic**

Computes average daily sales per product

Estimates days until stock-out

Classifies inventory risk:

HIGH – Less than 3 days

MEDIUM – 3 to 7 days

LOW – More than 7 days
