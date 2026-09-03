# EduPredict 🎓

### Early Academic Risk Prediction using Machine Learning

EduPredict is a machine learning project that identifies students who may be academically at risk using demographic, behavioral, social, and educational-support features.

## 🎯 Objective

The objective is to identify students who may be academically at risk at an early stage.

Students are classified using their final grade (`G3`):

- `0` → Not At Risk
- `1` → At Risk

The previous-period grades `G1` and `G2` were not used as input features.

## 📊 Dataset

- 649 student records
- 30 original features
- 17 categorical features
- 13 numerical features

The features include:

- Demographic information
- Study habits
- Family and social information
- School support
- Lifestyle-related attributes
- Absences

## ⚙️ Machine Learning Pipeline

Raw Dataset → Data Exploration → Target Creation → Train/Test Split → Feature Preprocessing → One-Hot Encoding + Scaling → Model Training → Model Evaluation

After preprocessing, the 30 original features were transformed into **56 machine-learning features**.

## 🤖 Models Tested

1. Logistic Regression
2. Decision Tree
3. Random Forest
4. Gradient Boosting

## 📈 Model Comparison

| Model | Accuracy | Precision | Recall | F1 Score |
|---|---:|---:|---:|---:|
| Logistic Regression | 76.92% | 35.29% | 60.00% | 44.44% |
| Decision Tree | 70.00% | 26.83% | 55.00% | 36.07% |
| Gradient Boosting | 83.08% | 41.67% | 25.00% | 31.25% |
| Random Forest | 80.77% | 33.33% | 25.00% | 28.57% |

## 🏆 Model Selection

Logistic Regression achieved the highest F1 score among the tested models and a recall of 60% for the At Risk class.

Although Gradient Boosting achieved higher accuracy, accuracy alone was not used for model selection because the dataset is imbalanced.

The project therefore gives particular importance to recall and F1 score for the At Risk class.

## 🔍 Model Interpretability

Logistic Regression coefficients were examined to identify features with stronger predictive associations.

Some influential features included:

- Previous failures
- Absences
- School-related attributes
- Higher-education preference
- Student-support variables
- Family and guardian-related attributes

These represent predictive associations in the model and should not be interpreted as causal relationships.

## 📊 Evaluation

The project uses:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC-AUC

## 🚀 Future Improvements

- Cross-validation
- Hyperparameter optimization
- More robust threshold selection
- Explainable AI techniques
- Interactive web deployment
- Testing on additional datasets

## 🛠️ Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## 👨‍💻 Author

ARJUN SINGH
