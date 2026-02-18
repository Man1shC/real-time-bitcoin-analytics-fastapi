# 🚀 Real-Time Bitcoin Analytics API

## 📌 Overview

This project is a production-style Bitcoin price analytics system built using FastAPI.  
It fetches real-time Bitcoin market data from the CoinGecko API, performs time-series analysis (including moving averages), and exposes RESTful endpoints for external consumption.

The application is containerized using Docker to enable scalable deployment.

---

## 🎯 Objective

To design and implement an end-to-end data pipeline that:

- Fetches live cryptocurrency market data  
- Performs analytical computations  
- Exposes results through REST APIs  
- Supports containerized deployment  

This project demonstrates backend engineering + applied data analytics.

---

## 🏗 System Architecture

```
Client
   ↓
FastAPI Server
   ↓
CoinGecko API
   ↓
Data Processing (Pandas)
   ↓
JSON Response
```

---

## ⚙️ Features

- Live Bitcoin price fetching  
- Historical price analysis  
- Simple Moving Average (SMA) calculation  
- REST API endpoints  
- Automatic API documentation via Swagger UI  
- Dockerized deployment  

---

## 📊 API Endpoints

| Endpoint | Method | Description |
|----------|--------|------------|
| `/price` | GET | Returns current Bitcoin price |
| `/history` | GET | Returns historical Bitcoin prices |
| `/moving-average` | GET | Computes moving average of prices |

---

## 🛠 Tech Stack

- Python  
- FastAPI  
- Pandas  
- Requests  
- SQLite (if applicable)  
- Docker  

---

## ▶️ Installation & Setup

### 1️⃣ Clone Repository

```bash
git clone https://github.com/Man1shC/real-time-bitcoin-analytics-fastapi.git
cd real-time-bitcoin-analytics-fastapi
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run Application

```bash
uvicorn main:app --reload
```

Open in browser:

```
http://127.0.0.1:8000/docs
```

---

## 🐳 Running with Docker

### Build Docker Image

```bash
docker build -t bitcoin-api .
```

### Run Container

```bash
docker run -p 8000:8000 bitcoin-api
```

---

## 📈 Future Improvements

- Add anomaly detection  
- Integrate LSTM-based forecasting  
- Add Redis caching layer  
- Deploy to AWS / GCP  

---

## 📌 Key Learnings

- Designing RESTful APIs  
- Integrating external APIs  
- Building scalable backend systems  
- Containerizing applications  
- Structuring production-ready repositories  

---

## 👨‍💻 Author

Manish Cheeti  
Machine Learning Engineer | Applied AI | Backend ML Systems
