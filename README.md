🫀 Predicting the Mortality of Heart Failure Patients

Machine Learning and Deep Learning project that predicts whether a heart failure patient will die during the follow-up period, using routine clinical records. Two models are built and compared: a Support Vector Machine (SVM) and an Artificial Neural Network (ANN).

📌 Problem Statement

Cardiovascular diseases are the leading cause of death worldwide, and heart failure is one of the most common outcomes. Early identification of high-risk patients helps doctors prioritise treatment. This project treats it as a binary classification problem:

0 → Patient survived
1 → Patient died (DEATH_EVENT)
📂 Dataset

Heart Failure Clinical Records Dataset (Chicco & Jurman, 2020; available on UCI ML Repository and Kaggle)

299 patients, 12 clinical features + 1 target
Collected at the Faisalabad Institute of Cardiology and Allied Hospital, Pakistan (2015)
Feature	Description
age	Age of the patient
anaemia	Decrease of red blood cells or haemoglobin (0/1)
creatinine_phosphokinase	Level of CPK enzyme in blood (mcg/L)
diabetes	Patient has diabetes (0/1)
ejection_fraction	% of blood leaving the heart at each contraction
high_blood_pressure	Patient has hypertension (0/1)
platelets	Platelets in blood (kiloplatelets/mL)
serum_creatinine	Level of creatinine in blood (mg/dL)
serum_sodium	Level of sodium in blood (mEq/L)
sex	Woman = 0, Man = 1
smoking	Patient smokes (0/1)
time	Follow-up period (days)
DEATH_EVENT	Target: death during follow-up (0/1)
🔄 Project Workflow
Import libraries: NumPy, Pandas, Matplotlib, Seaborn, scikit-learn, TensorFlow/Keras
Data analysis (EDA)
Class distribution of DEATH_EVENT
Correlation heatmap
Age vs death count
Swarm + boxen plots of key clinical features against the target
Preprocessing
Separate features (X) and target (y)
StandardScaler for feature scaling
70/30 train–test split
Model building
SVM with SVC() (default RBF kernel)
ANN (Keras Sequential): 16 → 8 → 8 → 1 neurons, ReLU activations, Dropout (0.25, 0.5), sigmoid output, Adam optimizer, binary cross-entropy loss, Early Stopping (patience = 20)
Evaluation using precision, recall, F1-score and accuracy (classification_report)
📊 Results
Model	Accuracy	Precision	Recall	F1-score
SVM	add	add	add	add
ANN	add	add	add	add

Fill in the numbers from your classification_report output. Results can change slightly between runs because the train–test split is random (set random_state for reproducibility).

🛠️ Tech Stack
Python 3
NumPy, Pandas
Matplotlib, Seaborn
scikit-learn
TensorFlow / Keras

🔮 Future Work
Hyperparameter tuning (GridSearchCV) for SVM and ANN
Try Random Forest, XGBoost, Logistic Regression for comparison
Handle class imbalance (SMOTE / class weights)
Cross-validation for more reliable evaluation
Feature importance / SHAP explainability
⚠️ Disclaimer

This project is for educational and research purposes only. It is not a medical diagnostic tool.
