# 🧑‍💼  Forecasting Workplace Absenteeism with Supervised Learning

This project analyzes employee absenteeism to uncover behavioral patterns and build predictive models that support workforce planning. Through data cleaning, exploratory analysis, and supervised learning, we aim to:

- Understand trends, seasonality, and key factors influencing absenteeism.
- Predict how many hours an employee is likely to be absent.
- Classify the employee's absence against the overall median.
- Compare linear and non-linear models to find the best predictive approach.

![image](https://github.com/user-attachments/assets/b56d5e4c-9d3c-4a38-a49b-84c849e7b46e)

## 🗃️ Dataset Overview

The dataset contains detailed absenteeism records for employees, including:

  - Demographics (age, education, family, smoking/drinking)
  - Work-related metrics (transport cost, service time, workload)
  - Time-based info (month, day of week, season)
  - Absence reasons (medical or non-medical)
  - Other variables

## 🛠️ Technologies
- pandas
- numpy
- matplotlib
- seaborn
- train_test_split
- LinearRegression, LogisticRegression
- RandomForestRegressor, RandomForestClassifier
- MAE, R2, Confusion Matrix, Accuracy, Recall, Precision, F1-Score
- ROC Curve, AUC Score

## 📈 Insights & Results

- Classification models are **more suitable** than regression for this data due to skew and discreteness.
- **Random Forest Classifier** provides the most robust predictions.
- `IsMedicalReason` is by far the most influential feature.
- Social behaviors (`IsDrinker`, `HasSon`, `HasPet`) also contribute meaningfully.


## 🧱 Workflow overview

### 1. Data Cleaning

- Removed 5.95% of entries where `Absenteeism time in hours = 0`.
- Corrected season labels by aligning them with the corresponding months.

### 2. Exploratory Data Analysis (EDA)

#### 📈 Quantitative Analysis

- Visualized distributions using **boxplots** and **density plots**.
- Key findings:
  - Absenteeism is **highly skewed**, mostly under 10 hours.
  - Most employees perform well (high `Hit target` scores).
  - Most employees have a relatively low workload
  - Some correlation expected between BMI, weight and height
  - Some correlation expected between age and service time.

#### 🚨 Outlier Detection

- Used **IQR method** to detect outliers in numerical features.
- Most outliers (especially in absenteeism) are **valid** and related to medical reasons.

#### 📊 Categorical Analysis

- Analyzed **value counts** and **countplots** for categorical features.
- Key findings:
  - **Seasonal peaks** in winter/spring and late summer.
  - Slightly higher absenteeism around **Mondays and Fridays**.
  - `Social drinker`, `Son`, and `Reason for absence` showed predictive potential.
  - `Disciplinary failure` has no predictive power.

#### ⚙️ Feature Engineering

- Created binary indicators:
  - `IsMedicalReason`, `IsEducation_Degree`, `HasSon`, `IsDrinker`, `IsSmoker`, `HasPet`
- Removed redundant categorical columns.

#### 📉 Correlation Analysis

- Computed correlation heatmap to identify relevant features.
- Selected 7 features with |corr| > 0.07 for modeling: `Distance from work`, `Height`, `IsMedicalReason`, `HasSon`, `Age`, `IsDrinker`, `HasPet`.


### 3. Regression Modeling (Log Target)

#### 🔹 Linear Regression

- Used log-transformed target to reduce skew.
- Model explained only **19% of variance (R² = 0.19)**.
- Residual plots showed non-random structure and **underprediction** of high values.
- The nature of the target variable significantly negatively affect the performance.

#### 🔸 Random Forest Regressor

- Prediction performance is roughly equal.
- **`IsMedicalReason`** was the most important feature by far.

### 4. Classification Modeling (Binary Target)

#### 🎯 New Target

- Created `Absenteism_Binary`: 1 if absence > median, else 0.
- The class imbalance is tiny.

#### 📉 Correlation Analysis
The feature selected with |corr| > 0.07 for modeling are: `Transportation expense`, `Service time`, `HitTarget`, `  IsMedicalReason`, `HasSon`, `IsDrinker`, `HasPet`.

#### 🔹 Logistic Regression

- The classification was iterated over different threshold probabilities.
- Best threshold for Accuracy (**0.72**) and F1 (**0.74**) is **P = 0.3**
- Best threshold for Recall (**0.91**): **P = 0.2**.
- Key coefficients impact:
  - Positive: `IsMedicalReason`, `HasSon`, `IsDrinker`
  - Negative: `HasPet`, `HitTarget`
- Evaluated residuals:
  - Binned residuals show random distribution


#### 🔸 Random Forest Classifier

- Trained with same features and grid search tuning.
- Best threshold for Accuracy (**0.76**) and F1 (**0.76**) is **P = 0.5**.
- Best threshold for Recall (**0.96**) is **P = 0.2**.
- Strongest features: `IsMedicalReason`, `HitTarget`, `Transportation expense`

#### 🆚 Logistic vs Random Forest comparison

| Metric      | Random Forest | Logistic Regression |
|-------------|---------------|---------------------|
| F1 Score    |  0.76        | 0.74                |
| Recall      | 0.78          | 0.82              |
| Precision   |  0.74        | 0.67                |
| Accuracy    |  0.76        | 0.72                |
| P           |  0.5         | 0.3                  |
| AUC         |  0.82        | 0.77                |

- ROC curves show similar ability to distinguish classes.
- **Random Forest** offers best balance between metrics.
- **Logistic** is slightly more interpretable and has higher recall.

## 📬 Contact
Feel free to connect with me on [Linkedin](https://www.linkedin.com/in/stefano-baglio/) or reach out via email at s.baglio.personal@outlook.com.


## 🗂️ Folder Structure

```bash
📁 supermarket-sales-analysis/
│
├── 📓 Forecasting_Workplace_Absenteeism_with_Supervised_Learning.ipynb
├── 📄 README.md
└── 📁 Data/


