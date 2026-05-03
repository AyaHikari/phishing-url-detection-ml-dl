# Phishing URL Detection using Machine Learning & Deep Learning Models

## Overview
Phishing attacks remain one of the most critical cybersecurity threats, targeting users through malicious URLs designed to steal sensitive information.  

This project implements and evaluates multiple **machine learning and deep learning models** to classify URLs as either *phishing* or *benign*. The goal is to analyze model performance and identify the most effective approach for real-world phishing detection systems.

## Objectives
- Detect phishing URLs using ML and DL models  
- Compare multiple classifiers for performance and efficiency  
- Evaluate models using standard metrics (Accuracy, Precision, Recall, AUC)  
- Analyze trade-offs between traditional ML and deep learning approaches  
- Visualize model behavior using ROC curves, confusion matrices, and learning curves  

## Models Implemented
The following models were implemented and evaluated:

- Random Forest (RF)  
- Fully Connected Neural Network (FCNN)  
- Long Short-Term Memory (LSTM)  
- Convolutional Neural Network (CNN)  

## Methodology

### 1. Data Preprocessing
- URL dataset containing phishing and benign samples
- Feature extraction from URLs
- Data cleaning and normalization

### 2. Model Training
Each model was trained on the processed dataset:
- Traditional ML: Random Forest
- Deep Learning: FCNN, LSTM, CNN

### 3. Evaluation Metrics
Models were evaluated using:
- Accuracy  
- Precision  
- Recall  
- F1 Score  
- AUC (ROC Curve Analysis)

### 4. Visualization Techniques
- ROC Curves  
- Confusion Matrices  
- Learning Curves  

## Results Summary

### Random Forest
- Accuracy: **87.15%**
- AUC: **~0.91–0.95**
- Fast training time (~0.59s)
- Strong overall balance of speed and performance

### Fully Connected Neural Network (FCNN)
- High precision and competitive accuracy
- Moderate training time (~10.8s)
- Good overall balance

### LSTM
- Good sequence learning capability
- Highest training time (~38.5s)
- Slight overfitting tendency observed

### CNN
- Strong generalization performance
- Balanced accuracy and training efficiency
- Stable learning behavior

## Key Insights

- **Random Forest** performed best in terms of efficiency and robustness  
- Deep learning models provided stronger representation power but required more computation  
- **CNN showed the best generalization among neural networks**  
- Ensemble and hybrid approaches have strong potential for future improvement  

## Evaluation Analysis

### ROC Curve Analysis
- Random Forest achieved the highest AUC score
- FCNN and CNN performed competitively
- LSTM showed slightly lower performance but remained effective

### Confusion Matrix Analysis
- Random Forest showed balanced classification performance  
- Neural networks showed slightly higher false positives/negatives depending on architecture  

### Learning Curves
- CNN demonstrated the most stable convergence  
- LSTM showed signs of overfitting  
- FCNN required tuning for better generalization  

## Tech Stack
- Python  
- Scikit-learn  
- TensorFlow / Keras  
- NumPy  
- Pandas  
- Matplotlib / Seaborn  

## Real-World Relevance
This project simulates real-world phishing detection systems used in cybersecurity environments such as SOCs (Security Operations Centers), where fast and accurate classification of malicious URLs is critical for threat prevention.

## Notes
This project is based on research exploring the sufficiency of ensemble machine learning methods for phishing website detection.
