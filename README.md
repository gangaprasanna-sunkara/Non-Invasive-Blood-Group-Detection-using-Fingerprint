# 🧬 Non-Invasive Blood Group Prediction Using Fingerprint Analysis

This repository contains the source code, training notebook, and demo system for my **Final Year Project (FYP)**:  
a **deep learning–based system** that predicts **blood groups from fingerprint images** using EfficientNet CNNs.  
It includes **model training**, a trained model, and a **Flask-based demo UI**.

---

---

## 📌 Project Overview
- **Goal**: Predict human blood groups using fingerprint images in a non-invasive manner.  
- **Dataset**: SOCOFing fingerprint dataset (synthetically labeled).  
- **Model**: EfficientNetB0 trained on 6,000+ fingerprint images across 8 blood groups.  
- **Accuracy**: Achieved **90.33% test accuracy**.  
- **Demo System**: Flask backend + HTML/CSS/JS frontend with a cyberpunk dark theme.  

⚠️ **Disclaimer**: This project is for **academic and research purposes only**. It is not medically validated and must not be used in real-world healthcare scenarios.

---

## 🛠 Tech Stack
- **Programming**: Python 3.10+, TensorFlow/Keras, scikit-learn, OpenCV  
- **Frontend**: HTML, CSS, JavaScript  
- **Backend**: Flask (API + templates)  
- **Visualization**: Matplotlib, Seaborn  
- **Deployment**: Local demo (Docker/Render compatible)  

---

## 📂 Project Structure
```

Non-Invasive-Blood-Group-Prediction-Using-Fingerprint-Analysis/
├── model/
│   ├── final_best_efficientnetb0_model_final.keras  # trained model (already included)
│   └── Model Training and Testing Code.ipynb                  # training & evaluation notebook
│
├── utils/                      # Helper scripts
│   └── predict.py              # Inference helpers
│
├── templates/                  # Flask HTML templates
├── static/                     # CSS, JS, sample input images
│
├── app.py                      # Flask backend for demo
├── requirements.txt            # Dependencies
├── README.md                   # Project description
├── LICENSE                     # MIT License
└── .gitignore                  # Ignore unnecessary files

````

---

## 🚀 Quickstart

### 1. Clone the repo
```bash
git clone https://github.com/wObbLee00/Non-Invasive-Blood-Group-Prediction-Using-Fingerprint-Analysis.git
cd Non-Invasive-Blood-Group-Prediction-Using-Fingerprint-Analysis
````

### 2. Create virtual environment & install requirements

```bash
python -m venv venv
# activate
venv\Scripts\activate  # Windows
source venv/bin/activate  # Linux/Mac
pip install -r requirements.txt
```

### 3. Model file
The trained model is **already included** in this repository at: `model/final_best_efficientnetb0_model_final.keras`
### 4. Run the demo

```bash
python app.py
```

* Open browser: `http://127.0.0.1:5000`

---

## 📊 Training

* Open `Model Training and Testing Code.ipynb` in Jupyter.
* Requires the SOCOFing dataset (not included due to size).
* Trains EfficientNetB0 with preprocessing, normalization, and dropout.
* Evaluated with accuracy, precision/recall, confusion matrix.

---

## 🎯 Features

* End-to-end ML pipeline: dataset → training → evaluation → deployment.
* Flask demo app with cyberpunk dark-themed UI.
* Easy to run locally (requirements + model file).
* Extendable to MLOps tools (Docker, MLflow, GitHub Actions).

---

## 📈 Results

* **Test Accuracy**: 90.33%
* **Model**: EfficientNetB0 (transfer learning)
* **Classes**: 8 blood groups → `['A+', 'A-', 'B+', 'B-', 'AB+', 'AB-', 'O+', 'O-']`

---

