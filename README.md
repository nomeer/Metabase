# Metabase

# 📊 Marketing Analytics Platform (Metabase + MySQL + ETL)

## 🚀 Overview

This project demonstrates an end-to-end **marketing analytics platform** integrating:

* 📢 Google Ads performance data
* 📩 Omnisend email marketing data
* 🛒 E-commerce order & revenue data

The system includes:

* Automated ETL pipelines
* Data warehouse (MySQL)
* Interactive dashboards (Metabase)

---

## 🧠 Business Objective

Enable marketing teams to:

* Track campaign performance across channels
* Measure engagement (CTR, CVR, ROAS)
* Understand customer behavior (new vs returning)
* Optimize ad spend and email campaigns

---

## 🏗️ Architecture

```text
Google Ads API ─┐
                ├── ETL Scripts (Python + Bash) ──> MySQL ──> Metabase Dashboards
Omnisend API ───┘
```

---

## ⚙️ Tech Stack

* **Database:** MySQL
* **BI Tool:** Metabase
* **ETL:** Python + Bash
* **APIs:**

  * Google Ads
  * Omnisend Statistics API

---

## 📊 Dashboards

### 📢 Google Ads Dashboard

* Impressions: **1.25M+**
* Clicks: **12.7K**
* Revenue: **$144K**
* ROAS tracking
* CTR, CVR, CPA trends

👉 Includes:

* Performance over time
* Product-level profitability
* Ad spend waste analysis

---

### 📩 Omnisend (Email Marketing)

* Emails Sent: **122K+**
* Opens: **37K+**
* Clicks: **1.9K+**
* Revenue tracking

👉 Includes:

* Campaign performance
* Engagement trends
* Subject line analysis

---

### 🛒 Revenue & Orders Dashboard

* Total Revenue: **$4.4M**
* Orders: **22K+**
* Avg Order Value: **$183.88**

👉 Includes:

* Revenue trends
* Orders over time
* Geographic performance (US map)
* New vs returning customers

---

## 📈 Key Insights

* 📊 Email campaigns drive high engagement but lower conversion rates
* 💰 Majority of revenue driven by repeat customers
* 📉 Some ad spend generates clicks without conversions (optimization opportunity)
* 📬 Campaign spikes directly impact revenue trends

---

## 🔄 ETL Pipeline

### Features:

* Incremental data sync using checkpoints
* API rate-limit handling
* Data normalization & transformation
* Daily aggregated statistics

### Example Pipelines:

* Google Ads → user segmentation (new vs returning)
* Omnisend → campaign + engagement stats
* Orders → customer lifecycle tracking

---

## 🧩 Data Models

Key tables:

* `google_ads_current`
* `google_ads_user_types`
* `omnisend_orders`
* `omnisend_daily_stats`
* `customer_first_order`

---

## 🔐 Security

Sensitive credentials are stored in `.env`:

```env
OMNISEND_API_KEY=your_api_key
DB_USER=your_user
DB_PASS=your_password
DB_HOST=your_host
DB_NAME=your_db
```

---

## 📸 Dashboard Preview
<img width="1066" height="863" alt="image" src="https://github.com/user-attachments/assets/d008bf52-5fbf-4230-af8c-ba56c64c9048" />

<img width="1058" height="551" alt="image" src="https://github.com/user-attachments/assets/a6ed04af-dd7c-45d9-988f-7801032c27fe" />

<img width="1106" height="740" alt="image" src="https://github.com/user-attachments/assets/af70c5df-5392-4c08-9805-20bf690968c7" />

<img width="1065" height="358" alt="image" src="https://github.com/user-attachments/assets/47585a14-99bb-400d-b160-306b0bc5537b" />

<img width="1118" height="661" alt="image" src="https://github.com/user-attachments/assets/d2864e07-c5d5-4f17-9663-c46e242bbe91" />



---

## 📂 Project Structure

```text
marketing-analytics/
 ├── etl/
 │    ├── omnisend_etl.py
 │    ├── google_ads.sql
 │    └── scripts.sh
 ├── dashboards/
 │    └── screenshots/
 ├── README.md
 └── .env.example
```

---

## 🧪 Future Improvements

* Add real-time streaming (Kafka / Airflow)
* Implement dbt for transformations
* Add predictive analytics (LTV, churn)
* Improve anomaly detection

---

## 👤 Author

Nomeer Sheikh

* GitHub: https://github.com/nomeer
* LinkedIn: https://linkedin.com/in/nomeer

---

## ⭐ Why This Project Stands Out

This project demonstrates:

* End-to-end data engineering + analytics
* Real-world marketing use cases
* API integration + ETL pipelines
* Business-focused dashboarding

---
