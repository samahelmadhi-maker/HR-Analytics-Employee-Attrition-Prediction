# HR-Analytics-Employee-Attrition-Prediction

## Overview

This project uses Machine Learning to predict employee attrition (employee turnover) using HR data.
The objective is to help HR teams identify employees at risk of leaving and support better retention strategies.

The notebook includes:

* Data cleaning and preprocessing
* Feature engineering
* Exploratory analysis
* Machine Learning modeling with Random Forest
* Threshold optimization
* Employee risk detection
* SMOTE balancing for imbalanced data
* CSV export for HR teams

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Imbalanced-learn (SMOTE)

---

## Project Structure

```bash
HR-Analytics-Employee-Attrition-Prediction/
│
├── HR_Analytics.ipynb
├── README.md
├── WA_Fn-UseC_-HR-Employee-Attrition.csv
└── employees_high_risk_attrition.csv
```

---

## Dataset

This project uses an HR employee attrition dataset containing information such as:

* Monthly income
* Work-life balance
* Distance from home
* Job satisfaction
* Overtime
* Years since last promotion
* Department
* Education
* Attrition status

Target variable:

* `Attrition` → Employee leaves or stays

---

## Machine Learning Workflow

### 1. Data Cleaning

* Removed unnecessary columns
* Converted target variable into binary format
* Checked missing values

### 2. Feature Engineering

Created additional business-focused features:

* Income level groups
* Distance risk category
* Work-life balance indicators

### 3. Encoding

* Ordinal encoding
* One-hot encoding for categorical variables

### 4. Model Training

Model used:

* Random Forest Classifier

Techniques:

* Train/Test split
* Cross-validation
* Class balancing

### 5. Evaluation Metrics

* ROC-AUC Score
* Classification Report
* Confusion Matrix
* Precision/Recall analysis

### 6. Threshold Optimization

The prediction threshold was adjusted to better detect employees at high risk of attrition.

### 7. SMOTE Balancing

SMOTE was applied to handle class imbalance and improve prediction quality.

---

## Results

The model identifies employees with a high probability of leaving the company.

Outputs include:

* Attrition probability score
* High-risk employee flag
* Exportable CSV file for HR decision-making

---

## Example Use Cases

* HR retention analysis
* Workforce planning
* Employee risk monitoring
* Business intelligence dashboards
* Predictive HR analytics

---

## How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/your-username/HR-Analytics-Employee-Attrition-Prediction.git
cd HR-Analytics-Employee-Attrition-Prediction
```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the notebook:

```bash
HR_Analytics.ipynb
```

---

## Future Improvements

* Deploy as a web application
* Add Power BI dashboard integration
* Compare multiple ML models
* Hyperparameter tuning
* Real-time prediction API

---

## Author

Samah Elmadhi

Data Analytics & Machine Learning Project
