# 💳 Suba Fintech — Next-Gen Digital Payments & Ambassador Platform

[![FastAPI](https://img.shields.io/badge/FastAPI-0.100+-009688?logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Alembic](https://img.shields.io/badge/Alembic-Migrations-d00000)](https://alembic.sqlalchemy.org/)
[![Railway Deployment](https://img.shields.io/badge/Deployed_on-Railway-0B0D0E?logo=railway&logoColor=white)](https://railway.app)

**Suba** is a comprehensive financial technology platform designed to facilitate instantaneous digital utility payments (Airtime, Data, Electricity bills) alongside an integrated Ambassador & Referral reward ecosystem. Built on high-concurrency asynchronous **FastAPI** architecture and structured web interfaces, Suba empowers everyday users and student brand ambassadors across Nigeria.

---

## ✨ Key Features

### ⚡ Digital Utility & Bill Payments (`wallet-core`)
- **Instant VTU Services**: Purchase airtime and high-speed data bundles across major Nigerian telecom providers (MTN, Airtel, Globacom, 9mobile).
- **Electricity & Cable Bills**: Token-based payment execution and verification flows (`buy-electricity.html`).
- **Secure Wallet Management**: Real-time wallet balances, transaction ledgers, and top-up tracking (`transactions.html`).

### 🏆 Ambassador & Leaderboard Dashboard
- **Referral Tracking Engine**: Real-time ambassador referral metrics, tier progression, and reward payouts (`ambassador.html`).
- **Live Leaderboard**: Dynamic widget ranking top-performing brand ambassadors with automated bonus allocations.

---

## 🛠️ Technology Stack

| Component | Framework / Tooling |
| :--- | :--- |
| **Backend API** | Python 3.12, FastAPI, Uvicorn (Asynchronous ASGI server) |
| **ORM & Database** | SQLAlchemy, Alembic Database Migrations, PostgreSQL |
| **Frontend UI** | Vanilla HTML5, CSS3, ES6 JavaScript, Responsive Flex/Grid layout |
| **Containerization** | Docker (`python:3.12-slim`), Railway / Render YAML specs |

---

## 🚀 Getting Started Locally

### Prerequisites
- **Python 3.12+**
- **Docker** (optional, for containerized execution)

### 1. Install Backend Dependencies
```bash
cd Suba/backend/suba
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### 2. Run Database Migrations
```bash
alembic upgrade head
```

### 3. Launch FastAPI Server
```bash
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```
Interactive OpenAPI documentation will be available at `http://localhost:8000/docs`.

### 4. Launch Frontend Web App
Serve the static HTML files using any local HTTP server:
```bash
cd Suba
python3 -m http.server 3000
```
Open `http://localhost:3000/index.html` in your web browser.

---

## 📄 License

Proprietary fintech infrastructure for **Suba Nigeria**. All rights reserved.
