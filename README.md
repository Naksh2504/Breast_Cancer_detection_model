# Breast Cancer Detection & Diagnostic System

An end-to-end machine learning web application for automated Fine Needle Aspirate (FNA) cytology nuclear morphometry analysis and risk prediction. The system combines a trained deep neural network with localized Shapley Additive Explanations (SHAP) for transparent, auditable diagnostic attribution.

---

## Features

- **30 Morphometric Cytology Inputs**: Standardized inputs covering Mean Nuclear Scale, Standard Error (cellular pleomorphism), and Extreme Atypia (worst characteristics).
- **Deep Neural Network Classification**: Calibrated neural network providing real-time malignancy risk stratification and confidence scoring.
- **Explainable AI (SHAP Attribution)**: Dynamic local feature attribution identifying the top physical drivers behind every prediction.
- **Single-Page Diagnostic Workstation**: Responsive White & Purple interface with sample test data loading and interactive model performance validation.

---

## Technical Stack

- **Backend**: Python 3.12, Flask, Flask-CORS
- **Deep Learning**: TensorFlow / Keras, Scikit-Learn
- **Explainability**: SHAP (Shapley Additive Explanations)
- **Frontend**: HTML5, Vanilla CSS, JavaScript, Chart.js

---

## Quickstart

### 1. Installation

```bash
# Clone the repository
git clone <your-repository-url>
cd Breast_Cancer_Detection-main

# Install dependencies
pip install -r requirements.txt
```

### 2. Run Locally

```bash
python app.py
```

The application will start at:
```
http://127.0.0.1:5000/
```

### 3. Usage

1. Open `http://127.0.0.1:5000/` in your browser.
2. Click **Test Data** to populate sample feature values, or enter custom cytometric measurements.
3. Click **Run Prediction** to generate the diagnostic assessment, risk probability, and SHAP attribution chart.
4. Scroll down to review the **Model Performance & Validation** confusion matrix and architectural specifications.

---

## Deployment

The application is structured for direct deployment on platforms such as Render, Railway, Heroku, or AWS:

- **Procfile** (for PaaS deployment):
  ```
  web: gunicorn app:app
  ```
- **Port Binding**: Uses standard host `0.0.0.0` and port `5000` (or `PORT` environment variable).

---

## Disclaimer

This system is an investigational decision-support tool designed for research and educational purposes. Automated predictions do not replace formal histopathological examination or clinical evaluation by licensed medical professionals.
