🧠 Cancer Detection ML Model

A machine learning project to classify breast cancer tumors as malignant or benign using diagnostic features from the Breast Cancer dataset.
---
❓ Problem Statement

Early detection of breast cancer is critical for improving survival rates. This project develops a machine learning pipeline that processes patient diagnostic data and predicts whether a tumor is cancerous or not.
---
📊 Dataset

Samples: 569

Features: 30 numerical attributes (cell nucleus characteristics)

Target:

M → Malignant (cancerous)

B → Benign (non-cancerous)
---
🚀 Workflow

flowchart TD
    A[Start] --> B[Import Libraries]
    B --> C[Load Dataset]
    C --> D[Explore Data]
    D --> E[Preprocess Data]
    E --> F[Split Features & Target]
    F --> G[Train-Test Split]
    G --> H[Feature Scaling]
    H --> I[Train Logistic Regression]
    I --> J[Evaluate Model]
    J --> L[Training Accuracy ~95%]
    J --> M[Test Accuracy ~94%]
    J --> N[Confusion Matrix]
    N --> O[Check Over/Underfitting]
    O --> P[Test on New Data]
    P --> Q[Prediction: Malignant/Benign]
    Q --> R[End]
---
📈 Result

Training Accuracy: ~99%

Test Accuracy: ~97%

Confusion Matrix: High precision & recall for both classes

Generalization: No overfitting → training and test performance are close
---
🧩 Code Breakdown

1. Import Libraries

Handles data, visualization, preprocessing, and model building.

2. Load & Explore Dataset

Read data.csv

Checked missing values

Previewed rows and data types

3. Preprocessing

Dropped irrelevant columns (id, Unnamed: 32)

Reordered columns to put diagnosis last

Normalized features with StandardScaler

4. Train-Test Split

80% training, 20% testing

Stratified sampling ensures balanced labels

5. Model Training

Algorithm: Logistic Regression

Fit on standardized training data

6. Model Evaluation

Compared training vs. test accuracy

Visualized results in a bar chart

Built confusion matrix

7. Performance Check

Overfitting/underfitting check based on score gap

8. Prediction on New Data

Input patient data vector

Predicted Malignant / Benign