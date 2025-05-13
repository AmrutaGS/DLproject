# Advanced Deep Learning Models for Mental Stress Classification Using GAF Encoding

Overview
This repository presents a deep learning-based approach to classify stress states using physiological time-series data. The raw data is first converted into Gramian Angular Field (GAF) images to preserve temporal information. The project implements and compares three deep learning architectures: an enhanced baseline Convolutional Neural Network (CNN), a hybrid CNN-Gated Recurrent Unit (CNN-GRU) model, and a Bidirectional Long Short-Term Memory (BiLSTM) network. These models are trained and evaluated on two well-known benchmark datasets — WESAD and SWELL — to identify and differentiate between various stress levels.

Repository Contents
This repository is organized into Jupyter notebooks, each dedicated to specific models or types of evaluation.

🔹 Core Notebooks (Per Model)
Each core notebook includes three primary components:

GAF Encoding: The time-series data from physiological signals is transformed into GAF images to capture temporal dynamics in a spatial format.

Model Architecture: The encoded images are used to train deep learning models — either CNN, CNN-GRU, or BiLSTM — optimized for classification tasks.

Evaluation Visualizations: Each notebook presents key visual analysis tools to assess performance, including:

Training and validation accuracy and loss curves,

Confusion matrix to evaluate prediction distributions,

Feature importance plots (e.g., SHAP or learned weights) to understand model decisions,

ROC curves to visualize classification thresholds and AUC.

These notebooks can be used for training and evaluation on both the WESAD and SWELL datasets.

🔹 Trend Analysis Notebooks (*_trend.ipynb)
The trend analysis notebooks are designed for in-depth performance diagnostics across different classes and models. They include:

Class-wise Performance Bar Graphs: These visualizations show how each model performs for each stress class in terms of accuracy, precision, recall, and F1-score.

Error-Based Evaluation Metrics: To further assess model performance, these notebooks compute:

Mean Absolute Error (MAE),

Mean Absolute Percentage Error (MAPE),

Root Mean Square Error (RMSE).

These metrics offer valuable insights into how well the models generalize and where they may underperform across the dataset classes.                                                         
Requirements
Python 3.x

Required Libraries:

TensorFlow 

NumPy

Matplotlib

OpenCV

scikit-learn
