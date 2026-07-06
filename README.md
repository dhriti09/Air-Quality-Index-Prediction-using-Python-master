# Air Quality Index Prediction System

This project is a full-stack Machine Learning web application designed to predict the **Air Quality Index (AQI)** based on real-time climate parameters. Developed as part of my B.Tech CSE curriculum at United Group of Institutions, this project implements a complete Data Science lifecycle.

## 🚀 Overview

The system predicts AQI by analyzing environmental factors such as temperature, humidity, and wind speed. It features a robust **Flask REST API** backend and a modern **React.js** frontend for a seamless user experience.

## 🛠️ Tech Stack

* **Frontend:** React.js
* **Backend:** Flask (Python)
* **Machine Learning:** Scikit-learn, XGBoost, Random Forest
* **Tools:** Git, VS Code, Jupyter Notebooks

## 📊 Project Lifecycle

### 1. Data Acquisition & Scrapping

Implemented a custom **Web Scraper** (`web_scrapper.py`) to extract historical climate data from *tutiempo.net*. The scraper processes monthly climate records and organizes them for further analysis.

### 2. Data Engineering & Cleaning

* Merged raw climate data with hourly AQI measurements.
* Handled missing values and outliers to ensure high data quality.
* **Preprocessing:** Created a unified CSV dataset by mapping daily climate features to AQI targets.

### 3. Model Building (Feature Engineering)

Experimented with multiple regression algorithms to find the most accurate predictor:

* Linear, Lasso, and Ridge Regression
* Decision Tree & KNN Regressors
* **Random Forest & XGBoost** (Top performing models)
* Final prediction is powered by **XGBoost Regressor** for its superior handling of non-linear environmental data.

## 💻 Local Setup

### Prerequisites

* Python 3.x
* Node.js (for Frontend)

### Steps

1. **Clone the Project**
```bash
git clone https://github.com/dhriti09/Air-Quality-Index-Prediction.git

```


2. **Setup Backend**
```bash
# Create and activate virtual environment
python -m venv venv
venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
python flask-app.py

```


3. **Setup Frontend**
```bash
cd aqi-frontend
npm install
npm start

```
