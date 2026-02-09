---

# Smart Grid Stability Prediction

Predicting the stability of smart grid systems is a crucial task for ensuring reliable and efficient power distribution in modern energy networks. This repository provides a complete machine learning workflow to analyze and classify the stability of smart grids using multiple feature selection techniques and ML models.

---

## 📌 Table of Contents

* 🔍 [Project Overview](#project-overview)
* 🗃 Repository Structure
* 🧠 ML Workflow
* 📊 Techniques & Models
* 🛠 Installation
* 🚀 Usage
* 📈 Sample Results
* 🤝 Contributing
* 📄 License

---

## 🔍 Project Overview

This project leverages classical machine learning methodologies to analyze and predict the stability of smart grid systems. Stability prediction helps operators take proactive measures to avoid outages, inefficiencies, and instability caused by fluctuations in load, generation, or grid configuration.

Smart grids generate data that can be used to train supervised models capable of distinguishing between *stable* and *unstable* states. This repository includes data preprocessing, feature selection, model training, and evaluation pipelines.

---

## 🗃 Repository Structure

```
Smart_Grid_Stability_Prediction/
├── PCA.ipynb                      # Principal Component Analysis workflow
├── RFE.ipynb                      # Recursive Feature Elimination workflow
├── Variance_Analysis.ipynb        # Variance threshold-based feature filtering
├── XGBOOST.ipynb                  # XGBoost model training & evaluation
├── svm,knn,dt,rf,lr.ipynb         # Multiple classical ML classifiers
├── Train.csv                      # Training dataset
├── Test.csv                       # Testing dataset
├── smart_grid_stability_augmented.csv
├── README.md                     # <— You are here!
```

---

## 🧠 ML Workflow

The project follows these steps:

1. **Data Loading & Exploration**
   Inspect dataset characteristics and class distributions.

2. **Feature Engineering & Preprocessing**
   Clean missing values, encode categories (if any), standardize/normalize features.

3. **Feature Selection Techniques**

   * **PCA (Principal Component Analysis)** — Dimensionality reduction
   * **RFE (Recursive Feature Elimination)** — Model-based selection
   * **Variance Analysis** — Remove low-variance features

4. **Modeling**
   Train multiple models such as Support Vector Machine (SVM), K-Nearest Neighbors (KNN), Decision Trees, Random Forest, Logistic Regression, and XGBoost.

5. **Evaluation**
   Evaluate performance using metrics like Accuracy, Precision, Recall, F1-Score, and Confusion Matrices across test sets.

---

## 📊 Techniques & Models

| Technique / Model       | Purpose                                                       |
| ----------------------- | ------------------------------------------------------------- |
| **PCA**                 | Reduce dimensionality for visualization and model performance |
| **RFE**                 | Identify best predictive features                             |
| **Variance Threshold**  | Filter out uninformative features                             |
| **SVM**                 | Classification with linear/nonlinear decision boundaries      |
| **KNN**                 | Instance-based classification                                 |
| **Decision Tree**       | Simple interpretable decision model                           |
| **Random Forest**       | Ensemble tree method for robustness                           |
| **Logistic Regression** | Baseline linear classifier                                    |
| **XGBoost**             | Boosted trees for high performance in tabular tasks           |

> Many of these approaches are also used in the broader literature for smart grid stability prediction with high accuracy and reliability. ([MDPI][1])

---

## 🛠 Installation

1. **Clone the repository**

   ```sh
   git clone https://github.com/Nirlova123/Smart_Grid_Stability_Prediction.git
   cd Smart_Grid_Stability_Prediction
   ```

2. **Create and activate a Python environment**

   ```sh
   python -m venv venv
   source venv/bin/activate      # macOS/Linux
   venv\Scripts\activate         # Windows
   ```

3. **Install dependencies**

   ```sh
   pip install -r requirements.txt
   ```

   If no `requirements.txt` exists, install common ML packages:

   ```sh
   pip install numpy pandas scikit-learn matplotlib xgboost seaborn notebook
   ```

---

## 🚀 Usage

1. Launch Jupyter Notebook:

   ```sh
   jupyter notebook
   ```

2. Open any of the provided `.ipynb` notebooks to explore:

   * PCA.ipynb
   * RFE.ipynb
   * svm,knn,dt,rf,lr.ipynb
   * XGBOOST.ipynb

3. Run cells in sequence to execute preprocessing, feature selection, model training, and evaluation.

---

## 📈 Sample Results

Each notebook saves visual outputs and evaluation metrics such as:

* Feature importance plots
* Model comparison charts
* Confusion matrices
* Classification reports

These help interpret model effectiveness and feature relevance.

---

## 🤝 Contributing

Contributions are welcome! You can:

* Add advanced models (e.g., deep learning)
* Improve preprocessing steps
* Add automated scripts for training & evaluation
* Write unit tests for functions

Please open issues or pull requests for enhancements.

---

## 📄 License

This project uses an open source license. See the `LICENSE` file for details.

---
