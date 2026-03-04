💳 Real-Time Fraud Detection System

> Detects fraudulent transactions in real-time using anomaly scoring, risk classification, and automated alert generation.

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-3.0-000000?style=for-the-badge&logo=flask&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-10b981?style=for-the-badge)

---

## ✨ Features

- **Transaction risk scoring** — amount, location, time, frequency
- **Alert levels: Safe / Low / Medium / High / Critical** — Alert levels: Safe / Low / Medium / High / Critical
- **Fraud analytics by merchant category and hour** — Fraud analytics by merchant category and hour
- **Automated alert creation for flagged transactions** — Automated alert creation for flagged transactions
- **REST API for real-time transaction ingestion** — REST API for real-time transaction ingestion

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Backend | Python 3.10+, Flask 3.x |
| Database | MySQL 8.x, mysql-connector-python |
| ML / NLP | Scikit-learn, Pandas, NumPy |
| Frontend | HTML5, CSS3, Chart.js, Jinja2 |

---

## 📁 Project Structure

```
fraud-detection/
├── app.py              ← Flask application + API routes
├── schema.sql          ← Database schema + seed data
├── requirements.txt    ← Python dependencies
├── .gitignore
├── LICENSE
└── templates/
    └── dashboard.html  ← Interactive dashboard UI
```

---

## ⚙️ Setup & Installation

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/fraud-detection.git
cd fraud-detection
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Configure database
Edit `DB_CONFIG` in `app.py`:
```python
DB_CONFIG = {
    "host":     "localhost",
    "user":     "your_mysql_user",
    "password": "your_mysql_password",
    "database": "fraud_db"
}
```

### 4. Initialize the database
```bash
mysql -u root -p < schema.sql
```

### 5. Run the application
```bash
python app.py
```

Visit: **[http://localhost:5010](http://localhost:5010)**

---

## 🗄️ Database Tables

```
transactions, fraud_alerts
```

---

## 🚀 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/` | Main dashboard |
| GET/POST | `/api/*` | REST API endpoints |
