# Medical-Diagnostic-Classification-Diabetes-

---
Diabetes Classification with Neural Networks

An end-to-end Machine Learning pipeline to predict diabetes diagnostics using clinical data. This repository demonstrates clean data engineering practices, handling datatype casting, and building a binary classification model using **TensorFlow/Keras 3** and **Scikit-Learn**.

---

Key Features
Data Engineering: Automated cleaning of biological inconsistencies (replacing invalid `0` values with feature-specific averages) while ensuring safe pandas datatype casting.
Feature Scaling: Normalized features using `StandardScaler` for stable gradient descent during neural network training.
Modern Keras Architecture: Built using the updated Keras 3 standards, defining input layers explicitly to guarantee environment compatibility.

---

Model Performance

The model delivers a solid and balanced baseline performance across both classes:

Test Accuracy: 72.73%

Classification Report
              precision    recall  f1-score   support

           0       0.79      0.79      0.79        99
           1       0.62      0.62      0.62        55

    accuracy                           0.73       154

```
Model Architecture

Input Layer: `keras.layers.Input` dynamically matching dataset features.
Hidden Layer 1: 16 Units with `ReLU` activation.
Hidden Layer 2: 8 Units with `ReLU` activation.
Output Layer: 1 Unit with `Sigmoid` activation for binary probability output.
Optimizer: `Adam` with `binary_crossentropy` loss.

---
Saved Production Artifacts

The pipeline automatically exports these production-ready files for deployment:

* `diabetes_model.keras` (The trained Deep Learning model)
* `scaler.pkl` (The configuration used to normalize user inputs)

---
How to Run

1. **Clone the repository:**
```bash
git clone [https://github.com/your-username/diabetes-classification.git](https://github.com/your-username/diabetes-classification.git)
cd diabetes-classification

```

2. **Install dependencies:**
```bash
pip install pandas numpy tensorflow matplotlib seaborn scikit-learn joblib

```


3. **Run the script/notebook:** Open your environment (VS Code or Jupyter) and execute the cells sequentially.

```
