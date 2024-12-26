# **Employee Burnout Prediction Project**

This repository contains a machine learning project aimed at predicting employee burnout rates based on various workplace and individual factors. The dataset used provides insights into organizational factors that influence employee mental health and burnout.

---

## **Table of Contents**
1. [Dataset Overview](#dataset-overview)  
2. [Project Objectives](#project-objectives)  
3. [Data Preprocessing](#data-preprocessing)  
4. [Models Used](#models-used)  
5. [Model Results](#model-results)  
6. [Installation & Usage](#installation--usage)  
7. [Key Visualizations](#key-visualizations)  
8. [Contributors](#contributors)

---

## **Dataset Overview**
- **Name**: Employee Burnout Analysis  
- **Source**: Uploaded internally for analysis.  
- **Features**:
  - `Date of Joining`: Employee's joining date.
  - `Resource Allocation`: Workload assignment.  
  - `Mental Fatigue Score`: Self-reported mental fatigue level.  
  - `Burn Rate`: Target variable representing employee burnout.  
  - `Gender`, `Designation`, `WFH Setup Available`, etc.  

- **Target Variable**: `Burn Rate`  
- **Missing Values**: Imputed using mean values for numerical features.  

---

## **Project Objectives**
1. Predict employee burnout rates accurately.  
2. Analyze factors contributing to burnout.  
3. Provide actionable insights for organizations to mitigate burnout.  

---

## **Data Preprocessing**
1. **Missing Values**:  
   - Imputed `Resource Allocation`, `Mental Fatigue Score`, and `Burn Rate` with their mean values.  

2. **Feature Engineering**:  
   - Label encoding for categorical variables (`Gender`, `Company Type`, `WFH Setup Available`).  
   - PCA applied for dimensionality reduction, retaining 95% of the explained variance.  

3. **Correlation Analysis**:  
   - Explored relationships between numerical features using heatmaps and plots.  

---

## **Models Used**
1. **Linear Regression**
2. **Random Forest Regressor**
3. **XGBoost Regressor**

---

## **Model Results**
| Model                   | R² Score  |
|--------------------------|-----------|
| **Linear Regression**    | 82.94%    |
| **Random Forest Regressor** | 83.89%    |
| **XGBoost Regressor**    | **85.30%** |

- **Best Model**: XGBoost Regressor with an R² score of 85.30%.  

---

## **Installation & Usage**
1. **Clone the Repository**:  
   ```bash
   git clone https://github.com/Riteshs677/employee-burnout-prediction.git
   cd employee-burnout-prediction
   ```

2. **Install Dependencies**:  
   Ensure you have Python 3.8+ and the required libraries installed.  
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Notebook**:  
   Open the Jupyter Notebook and execute the cells step by step:  
   ```bash
   jupyter notebook Employee_Burnout.ipynb
   ```

4. **Convert Notebook to PDF** (Optional):  
   Use the command below if LaTeX is installed.  
   ```bash
   jupyter nbconvert --to pdf Employee_Burnout.ipynb
   ```

---

## **Key Visualizations**
- **Correlation Heatmap**: Insights into relationships between features.  
- **Countplots**:
  - Distribution of `Gender`, `Company Type`, and `WFH Setup Available`.  
- **Burnout Trends**:
  - Burnout rates by `Designation` and `Mental Fatigue Score`.

---

## **Contributors**
- [Ritesh Singh](https://github.com/Riteshs677)  

Feel free to contribute or suggest improvements via pull requests.

---

## **License**
This project is licensed under the [MIT License](LICENSE).  
