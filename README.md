# Advanced Deep Learning Models for Mental Stress Classification Using GAF Encoding

## Overview

This repository presents a deep learning-based approach to classify stress states using physiological time-series data. The raw data is first transformed into **Gramian Angular Field (GAF)** images to preserve temporal patterns in a visual form. 

The project implements and compares four architectures:
- An enhanced baseline **Convolutional Neural Network (CNN)**
- A hybrid **CNN-Gated Recurrent Unit (CNN-GRU)** model
- A **Long Short-Term Memory (LSTM)** network
- A **Bidirectional Long Short-Term Memory (BiLSTM)** network

These models are trained and evaluated on two benchmark datasets — **WESAD** and **SWELL** — for identifying and differentiating between various mental stress levels.

---

## 📂 Repository Contents

This repository is organized into Jupyter notebooks, categorized based on model type and evaluation focus.

### Core Notebooks (Per Model)

Each core notebook includes:

- **GAF Encoding**: Time-series physiological signals are encoded into GAF images for spatial pattern recognition.
- **Model Architecture**: Deep learning models — CNN, CNN-GRU, LSTM, or BiLSTM — are implemented to perform classification.
- **Evaluation Visualizations**:
  - Accuracy and loss curves (training vs validation)
  - Confusion matrix
  - Feature importance plots (e.g., SHAP, gradient-based methods)
  - ROC curves with AUC

> These notebooks are compatible with both the **WESAD** and **SWELL** datasets.

---

### Trend Analysis Notebooks (`*_trend_.ipynb`)

These notebooks provide **in-depth model diagnostics**:

- **Class-wise Performance Visualizations**:
  - Bar graphs for class-wise accuracy, precision, recall, and F1-score
- **Regression Error Metrics**:
  - Mean Absolute Error (MAE)
  - Mean Absolute Percentage Error (MAPE)
  - Root Mean Square Error (RMSE)
These analyses offer deeper insights into each model's performance for every stress category and help identify patterns of over- or under-performance.
---
## Requirements

Make sure you are using **Python 3.x**.

### Required Libraries

Install the following dependencies to run the notebooks:
pip install tensorflow numpy matplotlib scikit-learn pandas seaborn pyts


