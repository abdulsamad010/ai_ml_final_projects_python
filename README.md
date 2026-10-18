<div align="center">

# 🚀 DevSphere Internship — Week 6 Final Project

### AI Intelligent Digit Recognition & ML House Price Prediction

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Machine_Learning-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)
[![Google Colab](https://img.shields.io/badge/Google_Colab-Notebook-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)](https://colab.research.google.com/)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/abdulsamad010)

**Prepared by:** Abdul Samad  
**Organization:** DevSphere  
**Repository:** `ai_ml_final_projects_python`

</div>

---

## 📌 Project Overview

This repository contains both Week 6 final projects in one Google Colab notebook, implemented with Python and Scikit-learn.

| Project | Objective | Dataset | Main Model |
|---|---|---|---|
| **Task 1 — AI** | Recognize handwritten digits and provide sample-based interaction | Scikit-learn Digits Dataset | Multi-Layer Perceptron Neural Network |
| **Task 2 — ML** | Predict median house values, compare models, and tune a regressor | California Housing Dataset | Linear Regression and Random Forest Regressor |

## 🧠 Task 1 — AI Intelligent Digit Recognition System

### Dataset
- **Dataset:** Scikit-learn Digits Dataset
- **Samples:** 1,797
- **Features:** 64 pixel values per sample
- **Image dimensions:** 8 × 8
- **Classes:** Digits 0–9
- **Training samples:** 1,437
- **Testing samples:** 360

### Workflow
1. Load and inspect the dataset, including the first five records.
2. Visualize class distribution and sample digit images.
3. Split data into training and testing sets using stratification.
4. Build a pipeline using `StandardScaler` and `MLPClassifier`.
5. Train the neural network and predict test labels.
6. Evaluate accuracy, precision, recall, F1 score, and the classification report.
7. Display the confusion matrix and training-loss curve.
8. Allow the user to select a test sample and view its predicted digit and confidence.

### Actual Results

| Metric | Recorded result |
|---|---:|
| Accuracy | **96.11%** |
| Weighted precision | **96.21%** |
| Weighted recall | **96.11%** |
| Weighted F1 score | **96.11%** |
| User-selected test sample | 300 |
| Actual digit | 5 |
| Predicted digit | 5 |
| Displayed confidence | **97.25%** |

### Task 1 Screenshots

Upload these image files to a `screenshots/` folder to make the following links render on GitHub.

**Dataset details and class distribution**

![Task 1 dataset details](screenshots/10001.PNG)

**Sample digit images and classification report**

![Task 1 samples and classification report](screenshots/1003.PNG)

**Confusion matrix and training loss**

![Task 1 confusion matrix and training loss](screenshots/1002.PNG)

**Sample prediction and user interaction**

![Task 1 user interaction](screenshots/1005.PNG)

**Dataset table preview**

![Task 1 dataset preview](screenshots/1004.PNG)

## 🏡 Task 2 — ML California House Price Prediction

### Dataset
- **Dataset:** California Housing Dataset from Scikit-learn
- **Samples:** 20,640
- **Features:** 8
- **Target:** Median house value in units of **$100,000**
- **Training samples:** 16,512
- **Testing samples:** 4,128

### Models and Workflow
- Compare **Linear Regression** and **Random Forest Regressor**.
- Use preprocessing pipelines and a train/test split.
- Tune the Random Forest model using `GridSearchCV` with 3-fold cross-validation.
- Evaluate models using R², mean absolute error (MAE), and root mean squared error (RMSE).
- Visualize target distribution, actual versus predicted values, and feature importance.
- Accept eight user-entered housing feature values for a prediction.

### Actual Results — Initial Comparison

| Model | R² Score | MAE | RMSE |
|---|---:|---:|---:|
| Linear Regression | 0.5758 | 0.5332 | 0.7456 |
| Random Forest | 0.8051 | 0.3275 | 0.5053 |

### Actual Results — Tuned Random Forest

| Metric | Recorded result |
|---|---:|
| Best cross-validation R² | **0.8012** |
| Test R² score | **0.8057** |
| MAE | **0.3266** |
| RMSE | **0.5046** |
| `max_depth` | `None` |
| `min_samples_leaf` | `2` |
| `n_estimators` | `120` |

### Sample Predictions

| Sample | Actual value | Predicted value |
|---|---:|---:|
| 1 | $47,700 | $50,128 |
| 2 | $45,800 | $77,323 |
| 3 | $500,001 | $488,297 |
| 4 | $218,600 | $254,309 |
| 5 | $278,000 | $233,950 |

The submitted user-input example used `33,44,55,66,77,11,55,66` and displayed **$320,256**. These values are not realistic for several housing features, so this output should be treated only as a software demonstration, not a meaningful real-world estimate.

### Task 2 Screenshots

**Dataset information and target distribution**

![Task 2 dataset and distribution](screenshots/2001.PNG)

**Initial model comparison and tuning results**

![Task 2 model comparison](screenshots/2002.PNG)

**Actual versus predicted house values**

![Task 2 actual versus predicted values](screenshots/2003.PNG)

**Feature importance and user prediction**

![Task 2 feature importance and user prediction](screenshots/2004.PNG)

## 🛠️ Technologies Used

- **Python** — implementation
- **Pandas and NumPy** — data inspection and numerical operations
- **Matplotlib** — graphs and visualizations
- **Scikit-learn** — datasets, preprocessing, pipelines, models, tuning, and evaluation
- **Google Colab** — notebook development and execution
- **GitHub** — repository hosting

## ▶️ How to Run

1. Open `AI_ML_Week6_Final_Project.ipynb` in Google Colab.
2. Run the Task 1 code cell and enter a test-sample number from 1 to 360 when prompted.
3. Run the Task 2 code cell. The California Housing dataset may need an internet connection on its first load.
4. Enter eight comma-separated numerical features in this order: `MedInc, HouseAge, AveRooms, AveBedrms, Population, AveOccup, Latitude, Longitude`.
5. Review the metrics, sample predictions, and visualizations.

## 🎯 Learning Outcomes

- Dataset inspection and exploratory visualization.
- Neural-network classification and regression workflows.
- Pipeline-based preprocessing and model training.
- Model evaluation using suitable classification and regression metrics.
- Cross-validation and hyperparameter tuning with GridSearchCV.
- Interpreting confusion matrices, loss curves, prediction plots, and feature importance.
- Implementing basic user interaction for model predictions.

## ⚠️ Notes

- Metrics are transcribed from the supplied notebook outputs and may vary if the code, data split, or library versions change.
- The digit-recognition project is an educational demonstration.
- House-price predictions are estimates, not guarantees or financial advice.
- Upload screenshots to a `screenshots/` folder with the exact filenames referenced above for GitHub image previews.

---

<div align="center">

**DevSphere Internship — Week 6 Final Project**  
*Consistent practice turns concepts into practical skills.*

</div>
