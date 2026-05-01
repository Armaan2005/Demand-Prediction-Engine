# 🚀 AI/ML Demand Prediction Engine

## 👨‍💻 Candidate Details

**Name:** Armaan Joshi

**Mobile:** 9079157371

---

## 📌 Project Overview

This project implements a **Demand Prediction Engine** that predicts how many units of a new product design will sell using:

* 📸 Product Design Images
* 📊 Historical Sales Data

The system combines **visual features + numerical data** and uses **ensemble machine learning models** to generate predictions.

---

## 🎯 Objective

To build a system that:

* Predicts product demand (quantity)
* Uses both image and tabular data
* Provides results through a working UI

---

## 🧠 Approach & Execution

### 1. Data Understanding

* Sales dataset includes:

  * Product code
  * Quantity sold
  * Price
  * Date
* ~180 product design images used

---

### 2. Data Preprocessing

* Cleaned missing values
* Structured dataset
* Prepared features for modeling

---

### 3. Feature Engineering

#### 📸 Image Features

* Extracted numerical representations from images
* Captured visual patterns influencing demand

#### 📊 Tabular Features

* Price-based features
* Historical demand signals

---

### 4. Feature Optimization

* Applied **StandardScaler** for normalization
* Used **PCA** to reduce dimensionality and noise

---

### 5. Model Building

Trained multiple regression models:

* Random Forest
* Gradient Boosting
* XGBoost

👉 Best model selected based on performance

---

### 6. Model Evaluation

Evaluation Metrics Used:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)

📊 **Model Performance (approx):**

* MAE: ~ low error range
* RMSE: optimized across models
* Best Model: XGBoost (highest accuracy)

---

### 7. Model Saving

* Saved trained models using:

  ```
  demand_prediction_models.pkl
  ```

---

### 8. UI (Working Interface)

* Built using **Gradio**
* User can:

  * Upload image
  * Enter price
  * Get predicted demand instantly

---

## ⚙️ How It Works

1. Upload product image
2. Enter price
3. Extract image features
4. Apply scaling + PCA
5. Model predicts demand
6. Output shown in UI

---

## 📂 Project Structure

```id="m6o2xe"
Demand-Prediction-Engine/
│
├── Demand_Prediction_Engine.ipynb
├── demand_prediction_models.pkl
├── sample_predictions.csv
├── eda_analysis.png
├── model_analysis.png
├── README.md
├── requirements.txt
```

---

## ⚙️ Setup Instructions

### 1. Clone Repository

```
git clone https://github.com/your-username/Demand-Prediction-Engine.git
cd Demand-Prediction-Engine
```

### 2. Install Dependencies

```
pip install -r requirements.txt
```

### 3. Run Notebook

* Open `Demand_Prediction_Engine.ipynb`
* Run all cells

### 4. Launch UI

* Execute UI cell (Gradio)
* Open generated public URL

---

## 🌱 Seed Script (Reproducibility)

To ensure consistent results:

```id="2r1rme"
import numpy as np
import random

np.random.seed(42)
random.seed(42)
```

---

## 📊 Sample Output

* Predictions stored in:

  ```
  sample_predictions.csv
  ```

---

## 🚀 Key Highlights

* End-to-end ML pipeline
* Image + tabular data fusion
* Ensemble models used
* Working UI
* Model persistence

---

## ⚠️ Limitations

* Limited dataset size
* Image feature extraction can be improved using CNN
* Model performance depends on data quality

---

## 🔮 Future Improvements

* Deep learning (CNN / ResNet)
* Hyperparameter tuning
* Cloud deployment
* Real-time predictions

---

## 📬 Submission Note

This project demonstrates:

* ML pipeline design
* Feature engineering
* Model building & evaluation
* UI integration

---
