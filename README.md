# Real-Time Sepsis Detection Using Machine Learning

## Overview

This project presents a machine learning approach for **early detection of sepsis** using real-time patient monitoring data. Sepsis is a life-threatening medical emergency, and timely identification is critical. Traditional scoring systems like SOFA and qSOFA are often limited in detecting early, subtle signs. This project leverages machine learning models—**Random Forest** and **XGBoost**—to enhance the accuracy and timeliness of detection using continuous ICU patient data streams.

## Objectives

- Develop machine learning models for real-time sepsis detection.
- Analyze and preprocess ICU data including vital signs and lab results.
- Evaluate model performance using AUC and precision-recall metrics.
- Compare results with clinical scoring systems (SOFA, qSOFA).
- Reduce false positives and support clinical decision-making.

## Research Questions

- How effective are Random Forest and XGBoost in detecting early sepsis compared to SOFA and qSOFA?
- What is the predictive performance in terms of AUC and precision-recall?
- How do the models reduce false positives and impact clinical interventions?

## Methodology

1. **Data Collection**  
   ICU data with patient vitals (heart rate, respiratory rate, temperature, BP) and lab results (e.g. lactate, WBC count).

2. **Data Preprocessing**  
   - Time series alignment  
   - Missing value handling  
   - Feature scaling and selection  

3. **Model Development**  
   - Random Forest  
   - XGBoost  
   - Hyperparameter tuning with cross-validation

4. **Evaluation Metrics**  
   - Area Under ROC Curve (AUC)  
   - Precision, Recall, F1-score  
   - Confusion Matrix

5. **Benchmarking**  
   Compare ML results with SOFA and qSOFA scoring accuracy.

## Technologies Used

| Technology     | Purpose                              |
|----------------|--------------------------------------|
| Python         | Core development                     |
| Scikit-learn   | Random Forest, preprocessing         |
| XGBoost        | Gradient boosting                    |
| Pandas, NumPy  | Data wrangling                       |
| Matplotlib     | Data visualization                   |
| Jupyter Notebook | Interactive development            |

## File Structure


## Installation

1. Clone the repository:
```bash
git clone https://github.com/Sravansai-2001/real-time-sepsis-detection-ml.git
cd real-time-sepsis-detection-ml
pip install -r requirements.txt
jupyter notebook notebooks/sepsis_model_training.ipynb
