# Heart Disease Prediction using Machine Learning and Deep Learning

## Overview
This project compares multiple **Machine Learning (ML)** and **Deep Learning (DL)** models for predicting the likelihood of heart disease based on clinical attributes such as age, cholesterol, and blood pressure.  
The work demonstrates how data preprocessing, feature scaling, and performance evaluation can be applied to healthcare analytics for early disease detection.

## Dataset
- **Source:** [UCI Machine Learning Repository – Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/heart+Disease)  
- **Samples:** 303 patient records  
- **Features:** 13 clinical attributes (e.g., `age`, `chol`, `thalach`, `trestbps`, `cp`)  
- **Target Variable:** `target` (1 = heart disease, 0 = no heart disease)

## Models Implemented
### Traditional Machine Learning Models
- Logistic Regression  
- Support Vector Machine (SVM)  
- Random Forest  
- XGBoost  

### Deep Learning Models (TensorFlow / Keras)
- Sequential Neural Network  
- Functional Neural Network  

## Evaluation Metrics
Each model was evaluated using:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **AUC (Area Under the ROC Curve)**

## Results Summary
| Model | Accuracy | Precision | Recall | F1-Score | AUC |
|:--|:--:|:--:|:--:|:--:|:--:|
| **Random Forest** | **0.820** | **0.762** | **0.970** | **0.853** | **0.912** |
| **Sequential Neural Network** | 0.787 | 0.763 | 0.879 | 0.817 | 0.884 |
| **Logistic Regression** | 0.803 | 0.769 | 0.909 | 0.833 | 0.869 |
| **Support Vector Machine** | 0.803 | 0.778 | 0.848 | 0.812 | 0.887 |
| **Functional Neural Network** | 0.820 | 0.789 | 0.909 | 0.84 | 0.883 |
| **XGBoost** | 0.770 | 0.757 | 0.848 | 0.800 | 0.859 |

**Best Model:** Random Forest  
Random Forest and Functional Neural Networks achieved the highest overall performance, showing strong generalization on the test data espcially on the acurracy.

## Insights
- Ensemble tree models (Random Forest) outperform deep models on small tabular data.  
- Neural Networks show potential but are more sensitive to data size and regularization.  
- Feature scaling and dropout regularization significantly impact model stability and performance.  

## How to Run
1. Clone the repository:  
   ```bash
   git clone https://github.com/<your-username>/heart-disease-prediction.git
   cd heart-disease-prediction
