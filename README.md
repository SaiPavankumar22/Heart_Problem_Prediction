# Heart_Problem_Prediction

## Overview
This project focuses on predicting the likelihood of heart disease based on a variety of medical and personal health indicators. Using machine learning techniques, it aims to create a reliable and interpretable model to assist in early detection of heart disease.

### Features
- Implementation of multiple classification models: knn, Decision Tree, Random Forest, Support Vector Machine (SVM).
- Hyperparameter tuning for optimizing model performance.
- Dynamic input functionality to allow users to predict heart disease for custom inputs.
- Visualization of the dataset to understand relationships between features and target labels.

---

## Dataset
The dataset used includes the following features:
- **Age**: Age of the patient.
- **Sex**: Gender of the patient (0 for Female, 1 for Male).
- **ChestPainType**: Type of chest pain (`ATA`: 0, `NAP`: 1, `ASY`: 2, `TA`: 3).
- **RestingBP**: Resting blood pressure (in mm Hg).
- **Cholesterol**: Serum cholesterol level (in mg/dl).
- **FastingBS**: Fasting blood sugar level (1 if > 120 mg/dl, 0 otherwise).
- **RestingECG**: Resting electrocardiographic results (`Normal`: 0, `ST`: 1, `LVH`: 2).
- **MaxHR**: Maximum heart rate achieved.
- **ExerciseAngina**: Exercise-induced angina (0 for No, 1 for Yes).
- **Oldpeak**: ST depression induced by exercise relative to rest.
- **ST_Slope**: Slope of the peak exercise ST segment (`Up`: 0, `Flat`: 1, `Down`: 2).
- **HeartDisease**: Target variable (1 indicates presence, 0 indicates absence).

---

## Implementation
1. **Data Preprocessing**:
   - Missing value handling and encoding of categorical variables.
   - Splitting the data into training and testing sets.
2. **Model Training**:
   - Trained models including Logistic Regression, Random Forest, SVM, and Decision Tree.
   - Hyperparameter tuning using GridSearchCV.
3. **Evaluation**:
   - Compared models based on accuracy scores.
   - Selected the model with the highest accuracy as the best predictor.
4. **Dynamic Prediction**:
   - A function that takes user inputs dynamically to predict the target variable.

---

## Visualizations
Key insights were derived using:
- Bar plots to analyze the distribution of features such as gender, chest pain type, etc.
- Correlation heatmaps to evaluate relationships between features.
- Violin plots and other advanced visualizations for in-depth analysis.

---

## Instructions
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/heart-disease-prediction
   ```
2. **Install Dependencies**:
   - Ensure Python 3.x is installed.
   - Install required libraries:
     ```bash
     pip install -r requirements.txt
     ```
3. **Run the Model**:
   - Execute the notebook to train models and visualize the data.
4. **Dynamic Prediction**:
   - Use the `predict_heart_disease()` function for real-time predictions.

---

## Input Requirements for Prediction
- **Age**: Integer.
- **Sex**: 0 (Female) or 1 (Male).
- **ChestPainType**: 0 (ATA), 1 (NAP), 2 (ASY), 3 (TA).
- **RestingBP**: Positive integer.
- **Cholesterol**: Positive integer.
- **FastingBS**: 0 or 1.
- **RestingECG**: 0 (Normal), 1 (ST), 2 (LVH).
- **MaxHR**: Positive integer.
- **ExerciseAngina**: 0 (No), 1 (Yes).
- **Oldpeak**: Float.
- **ST_Slope**: 0 (Up), 1 (Flat), 2 (Down).

---

## Future Enhancements
- Deploy the model as a web application.
- Add additional machine learning techniques.
- Integrate real-world datasets for model improvement.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---
