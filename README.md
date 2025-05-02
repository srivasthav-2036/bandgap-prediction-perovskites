#  Band Gap Prediction of Perovskite Oxides using Machine Learning

This repository contains a machine learning-based solution to predict the **band gap (Eg)** of **Perovskite oxides**, a class of materials critical to next-generation electronics like solar cells, LEDs, and semiconductors.

##  Problem Statement

Perovskite oxides have tunable electronic properties, and accurately predicting their band gap helps in material discovery for electronic and optoelectronic applications. Traditional methods can be slow and computationally expensive, so this project uses machine learning to predict band gaps quickly and efficiently.

---

##  Project Structure

- `Copy_of_Notebook.ipynb`: Jupyter notebook with data preprocessing, feature engineering, model training, and evaluation.
- `Report_Composit_Excavate.pdf`: A detailed project report including methodology, insights, and model performance.


---

##  Dataset Overview

- **Total Rows**: 5151  
- **Columns**: 38  
- **Data Types**: 30 float, 3 int, 5 object  
- **No missing values**

---

##  Machine Learning Models

### 1.  XGBoost Classifier

- **Purpose**: Classify materials as insulators or not based on band gap.
- **Hyperparameters**:
  - `n_estimators`: 10
  - `criterion`: entropy
  - `random_state`: 42
  - `max_cat_threshold`: 20
- **Performance**:
  - **Accuracy**: 0.9992

### 2.  Random Forest Regressor

- **Purpose**: Predict the exact numerical value of the band gap.
- **Hyperparameters**:
  - `n_estimators`: 250
  - `max_depth`: 8
  - `random_state`: 42
- **Performance**:
  - **Mean Squared Error (MSE)**: 0.155
  - **R² Score**: 0.751

---

##  Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Perovskite-BandGap-Prediction.git
   cd Perovskite-BandGap-Prediction
   ```

2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the notebook:
   ```bash
   jupyter notebook New_Copy_of_Notebook.ipynb
   ```

##  Prerequisites

Make sure you have the following installed:

- Python 3.8 or above
- Jupyter Notebook or JupyterLab
- pip (Python package manager)

##  Dependencies

Install the required Python packages:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
```
