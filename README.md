# Student Depression Dataset Analysis

## Project Overview
The primary goal of this project is to analyze a student depression dataset and predict whether a student is depressed or not. Two models, Logistic Regression and Decision Tree, are applied and evaluated based on their accuracy. Additionally, the impact of outlier removal on model performance is investigated.

---

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Dataset Details
The dataset includes features such as:
- Age
- Academic Pressure
- Work Pressure
- CGPA
- Job Satisfaction
- Depression (Target Variable: 0 or 1)

The target variable indicates whether a student is depressed (1) or not (0).

---

## Steps Performed

### 1. Exploratory Data Analysis (EDA)
- Visualized the dataset using pair plots and box plots to identify patterns and relationships between features.
- Checked for outliers using box plots.
- Analyzed correlations between numerical features using a heatmap.

### 2. Model Implementation
#### a) Logistic Regression
- Split the dataset into training and testing sets.
- Applied Logistic Regression.
- Achieved an accuracy of **83%** before removing outliers.

#### b) Decision Tree Classifier
- Implemented a Decision Tree model.
- Achieved an accuracy of **76%** before removing outliers.

### 3. Outlier Removal
- Identified outliers using the Interquartile Range (IQR) method for numerical features such as 'Age','Job Satisfaction' and 'Study Satisfaction'.
- Removed outliers from the dataset.
- Re-evaluated the Logistic Regression model on the cleaned dataset.
- Achieved an improved accuracy of **84%** after outlier removal.

---

## Results
| Model                | Accuracy (Before Outlier Removal) | Accuracy (After Outlier Removal) |
|----------------------|-----------------------------------|---------------------------------|
| Logistic Regression  | 83%                               | 84%                              |
| Decision Tree        | 76%                               | Not Evaluated                    |

---

## Conclusion
- Logistic Regression performed better than the Decision Tree model in predicting depression in students.
- Outlier removal improved the Logistic Regression model's accuracy slightly, from **83% to 84%**.
- EDA and proper data preprocessing, including handling outliers, are crucial steps in improving model performance.

---

## Future Work
- Evaluate the Decision Tree model after outlier removal.
- Experiment with other models, such as Random Forest or Gradient Boosting.
- Perform feature engineering to identify additional impactful features.

---

