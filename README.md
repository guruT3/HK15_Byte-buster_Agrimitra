This is the disease detection model, the file size was large so we didn't upload it so download it from here by going to given 
link:  https://drive.google.com/file/d/1cSmE7VI9FDIKPGe1bxQGM0fLrig0NAfC/view?usp=drive_link













# 🌾 Agri Mitra – Smart Digital Companion for Every Farm

> **"AI Copilot for Intelligent Farm Operations & Decision Execution"**

[![HackNovation 2.0](https://img.shields.io/badge/HackNovation-2.0-green)](https://www.giet.edu)
[![Team](https://img.shields.io/badge/Team-Byte%20Busters-blue)]()
[![Problem Statement](https://img.shields.io/badge/Problem%20Statement-HK--15-orange)]()

---

## 📌 Overview

**Agri Mitra** is an AI-powered smart farming platform designed to bridge the gap between fragmented agricultural data and real, actionable guidance for farmers. By combining crop prediction, disease detection, real-time weather forecasting, market price analysis, and multilingual AI support into a single ecosystem, Agri Mitra empowers farmers to make data-driven decisions every day.

---

## 🚜 Problem Statement

Agriculture supports over 58% of India's population, yet farmers — especially the 80% who are small and marginal — lack access to real-time digital decision support. Critical challenges include:

- Unpredictable weather patterns affecting crop planning
- Rapid spread of crop diseases without early detection
- Volatile market prices and poor market access
- Fragmented apps offering isolated, incomplete solutions

**There is a clear need for a unified, AI-driven system that converts raw farm data into simple, explainable daily action plans.**

---

## 💡 Proposed Solution

Agri Mitra processes farmer inputs (soil data, location, crop images, and specific requirements) through a suite of AI/ML models and delivers personalized recommendations and action plans.

**Technology Stack:**
- Machine Learning models for crop prediction
- Convolutional Neural Networks (CNN) for disease detection (99%+ accuracy)
- Real-time Weather API integration
- Market Data Analytics for price trend prediction
- Multilingual AI Chatbot (Hindi, Odia, Telugu, and more)

**Flow:**
```
Farmer Input → AI Processing (ML Models + APIs) → Personalized Recommendation & Action Plan → Improved Productivity & Profit
```

---

## ✨ Features

### Current Features
| Unique Features | Standard Features |
|---|---|
| Credit & gamification system | Disease prediction |
| 7-day personalized farming plan | Accurate crop prediction |
| Job portal for agri-workers | Smart Farm Calendar |
| Field analysis & appointment booking | Agricultural Calculator |
| Cold storage locator | Weather Forecast |
| Market price analysis | Community & contact forum |
| Courses & agri-games | Loan Assistant |
| Multi-language AI Chatbot | EMI Calculator |

### Upcoming Features
- Drone-based field scanning & IoT monitoring
- AI-powered yield and price prediction at scale
- Voice-based assistance for easy navigation
- Offline mode for low-network rural areas
- USSD/IVR support for feature phone users

---

## 📊 Market Opportunity

| Segment | Size |
|---|---|
| TAM – All farmers globally | ~570 million |
| SAM – Indian farmers with smartphone access | ~150+ million |
| SOM – Target in first 3–5 years | 5–10 million |

**Key Competitors:** DeHaat, AgroStar, Ninjacart, Kisan Suvidha

**Our Edge:** Agri Mitra is India's first integrated AI-powered farming ecosystem combining crop advisory, disease detection, financial assistance, an IoT marketplace, and a farmer social network — all in one platform.

---

## 🗺️ Go-To-Market Strategy

1. **Pilot Launch** – Deploy in one agriculture-dominant district, partnering with local FPOs and Krishi Vigyan Kendras (KVKs)
2. **Community Onboarding** – Village awareness camps, WhatsApp-based onboarding, and referral rewards
3. **Strategic Partnerships** – Agri-input suppliers, rural banks, microfinance institutions, and government agriculture departments
4. **Scale** – District → State → Multi-state expansion with added regional language support

---

## 💰 Business Model

- **Freemium Subscriptions** – Basic advisory free; premium AI insights paid
- **IoT Marketplace Commission** – 5–10% on transactions
- **Job Portal Placement Fees**
- **B2B SaaS** – For FPOs and agri-corporates
- **Future:** Government contracts, loan referral fees, and ad revenue from agri-brands

---

## 🛣️ Roadmap

- [x] Crop prediction ML model
- [x] Disease detection CNN model (99%+ accuracy)
- [x] Multilingual AI chatbot (Hindi, Odia, Telugu)
- [x] 7-day personalized farm plan generator
- [x] Smart Farm Calendar & Agri Calculator
- [x] Weather API integration
- [x] Market price data integration
- [ ] Drone & satellite field analysis integration
- [ ] Real-time IoT sensor data processing
- [ ] Government scheme & subsidy alert integration
- [ ] Offline mode for rural connectivity

---

## 🚀 Getting Started

Follow these steps to clone, set up, and run Agri Mitra locally on your machine.

### ✅ Prerequisites

Make sure you have the following installed before you begin:

- [Python 3.9+](https://www.python.org/downloads/)
- [Git](https://git-scm.com/)
- `pip` (comes with Python)

You can verify your installations by running:

```bash
python --version
pip --version
git --version
```

---

### 📥 Step 1 – Clone the Repository

```bash
git clone https://github.com/your-username/agri-mitra.git
cd agri-mitra
```

---

### 🐍 Step 2 – Create a Virtual Environment

It's recommended to use a virtual environment to keep dependencies isolated.

```bash
# Create the virtual environment
python -m venv venv

# Activate it — on Windows:
venv\Scripts\activate

# Activate it — on macOS/Linux:
source venv/bin/activate
```

---

### 📦 Step 3 – Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 🗄️ Step 4 – Set Up the Database

Agri Mitra uses **SQLite3**, which requires no external setup. Just run the following command to initialize the database and create all required tables:

```bash
python setup_db.py
```

This will generate a `agrimitra.db` file in your project directory automatically.

---

### 🔑 Step 5 – Configure Environment Variables

Create a `.env` file in the root of the project and add your API keys:

```bash
cp .env.example .env
```

Then open `.env` and fill in your values:

```env
FLASK_APP=app.py
FLASK_ENV=development
SECRET_KEY=your_secret_key_here
WEATHER_API_KEY=your_openweather_api_key
MARKET_API_KEY=your_market_data_api_key
```

> 💡 You can get a free Weather API key from [OpenWeatherMap](https://openweathermap.org/api).

---

### ▶️ Step 6 – Run the Application

```bash
flask run
```

The app will start on **http://127.0.0.1:5000** by default. Open this URL in your browser to access Agri Mitra.

---

### 🤖 Step 7 – Run the AI Models (Optional)

To test the crop prediction and disease detection models independently:

```bash
# Run crop prediction model
python models/crop_prediction.py

# Run disease detection model
python models/disease_detection.py
```

---

### 🧪 Running Tests

```bash
pytest tests/
```

---

### 📁 Project Structure

```
agri-mitra/
│
├── app.py                  # Main Flask application entry point
├── setup_db.py             # Database initialization script
├── requirements.txt        # Python dependencies
├── .env.example            # Environment variable template
│
├── models/                 # AI/ML model scripts
│   ├── crop_prediction.py
│   └── disease_detection.py
│
├── static/                 # CSS, JS, images
├── templates/              # HTML templates (Jinja2)
├── routes/                 # Flask route blueprints
├── database/               # SQLite3 DB and schema files
└── tests/                  # Unit and integration tests
```

---


**Port already in use?**
```bash
flask run --port 5001
```

**Module not found errors?**
Make sure your virtual environment is activated and dependencies are installed:
```bash
source venv/bin/activate   # or venv\Scripts\activate on Windows
pip install -r requirements.txt
```

**Database errors?**
Delete the existing `.db` file and re-run setup:
```bash
rm agrimitra.db
python setup_db.py
```

---

## 👥 Team – Byte Busters

| Name | Roll No. | Semester |
|---|---|---|
| Guru Prasad Palai | 24CSE102 | 4th Sem, CSE |
| Milind Panda | 24CSE097 | 4th Sem, CSE |
| Jashobanta Sasmal | 24CSE070 | 4th Sem, CSE |

> Built for **HackNovation 2.0** — R&D Cell, GIET University, Gunupur



*Made with ❤️ for India's farmers*
