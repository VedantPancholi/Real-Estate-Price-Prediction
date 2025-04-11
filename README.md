# 🏡 Real Estate Price Prediction using Machine Learning (Deployed on AWS EC2)

This repository contains a **Machine Learning model** that predicts real estate prices based on various property features such as location, size, and amenities. The project includes **data preprocessing, feature engineering, model training, and evaluation** to ensure an accurate and reliable price prediction model. It is also **deployed on an AWS EC2 Ubuntu instance**, accessible via public DNS.

---

## 📌 Table of Contents
- [Introduction](#introduction)
- [Project Workflow](#project-workflow)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Model Training](#model-training)
- [Results](#results)
- [How to Run the Project](#how-to-run-the-project)
- [EC2 Deployment Guide](#ec2-deployment-guide)
- [Directory Structure](#directory-structure)
- [Future Enhancements](#future-enhancements)
- [Contributors](#contributors)

---

## 🔍 Introduction

Predicting property prices is essential for real estate buyers, sellers, and investors. This project aims to:

- Analyze key factors influencing property prices.
- Build a robust ML model to predict real estate prices.
- Provide valuable insights into real estate trends.

The model is trained using **machine learning techniques**, with an emphasis on **data cleaning, feature selection, and hyperparameter tuning**.

---

## 🛠 Project Workflow

1. **Data Collection** - Collect real estate data containing various property attributes.
2. **Data Preprocessing** - Handle missing values, encode categorical features, and scale numerical data.
3. **Feature Engineering** - Select the most relevant features for the model.
4. **Model Selection & Training** - Compare different ML models (Linear Regression, Decision Trees, XGBoost, etc.).
5. **Hyperparameter Tuning** - Optimize the model for better performance.
6. **Evaluation & Predictions** - Assess model accuracy using performance metrics.
7. **Deployment** - Deploy the model using Flask API on AWS EC2.

---

## 📊 Dataset

- **Features Included:**
  - `Location`, `Size`, `Bedrooms`, `Bathrooms`, `Age`, `Amenities`, `Price`
- **Preprocessing:**
  - Handle missing values
  - Encode categorical variables
  - Scale features using MinMaxScaler/StandardScaler

---

## 💻 Technologies Used

- **Languages:** Python 🐍
- **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`
- **API Framework:** Flask
- **Deployment:** AWS EC2, Ubuntu, Nginx, Gunicorn, Putty, WinSCP

---

## 🏗️ Model Training

The following models were tested:

1. **Linear Regression**
2. **Decision Tree Regressor**
3. **Random Forest Regressor**
4. **XGBoost Regressor** (Final Model)

- **Best Model Selection Criteria:**
  - Higher **R² score** (explains variance in data)
  - Lower **RMSE** (Root Mean Squared Error)
  - Robustness against overfitting

- **Final Model Used:** **XGBoost Regressor**
- **Hyperparameter Tuning Method:** Grid Search / Random Search

---

## 📊 Results

- **Key Insights:**
  - Location and Size had the highest feature importance.
  - Model generalized well on unseen data.

---

## 🚀 How to Run the Project

### Step 1: Clone the Repository
```bash
git clone https://github.com/Mansi111000/Real_Estate_Price_Prediction_ML.git
cd Real_Estate_Price_Prediction_ML
```

### Step 2: Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 3: Run the Model
```bash
python train_model.py
```

### Step 4: Make Predictions
```bash
python predict.py --input sample_data.csv
```

---

## ☁️ EC2 Deployment Guide

- Launch EC2 Ubuntu instance
- Allow inbound rules: **SSH, HTTP, HTTPS**
- Generate `.pem` key → convert to `.ppk` using **PuTTYgen**
- SSH into instance via Git Bash:
```bash
ssh -i <path-to-pem> ubuntu@<public-dns>
```

### WinSCP Setup:
- Host: Public DNS of EC2
- Username: `ubuntu`
- Auth: Add `.ppk` in Advanced > SSH > Authentication

### Web Server Setup:
- Install NGINX & Python3 venv
- Navigate to `/var/www/html` or redefine root in `bhp.conf`
- Activate your virtual environment:
```bash
cd BHP/server
source venv/bin/activate
python3 server.py
```

### Access the Server:
- Copy EC2 **Public DNS** in browser after server runs
- You’ll see your deployed app live on the internet ✅

---

## 👤 Directory Structure

```bash
Real_Estate_Price_Prediction_ML/
├── data/
├── notebooks/
├── models/
├── scripts/
│   ├── preprocess.py
│   ├── train_model.py
│   ├── predict.py
├── app/
├── config.yaml
├── README.md
```

---

## 🔮 Future Enhancements

- Improve Feature Engineering
- Try Deep Learning models (ANNs)
- Integrate Real-Time APIs
- Deploy with Docker & CI/CD pipelines

---

## 👥 Contributors

- **Mansi111000** - [GitHub Profile](https://github.com/Mansi111000)
- **VedantPancholi** - [GitHub Profile](https://github.com/VedantPancholi)

> ⭐ Feel free to fork, star, and contribute!



