# Heart_disease_analysis_-
The dataset contains medical attributes related to heart disease, including:

Age (age)
Cholesterol (chol)
Resting Blood Pressure (trestbps)
Maximum Heart Rate (thalach)
Chest Pain Type (cp)
ECG Results (restecg)
Target (Heart Disease Presence) (target)
-------------------------------------------------------------------------------------------------------------------------
🛠 Features & Steps
1️⃣ Data Loading & Preprocessing (Pandas)
* Load the dataset
* Display columns, head & tail, and descriptive statistics
* Handle missing values using mean imputation
* Identify and remove outliers
* Check dataset shape before & after processing
2️⃣ Numerical Analysis (NumPy & Pandas)
* Compute mean, median, standard deviation of key indicators
* Analyze blood pressure based on heart disease presence
* Sort and search patients based on cholesterol & age
* Reshape and split data using NumPy
  ----------------------------------------------------------------------------------------------------------------------------
3️⃣ Data Visualization (Matplotlib & Seaborn)
📌 Histogram: Cholesterol distribution
📌 Scatter Plot: Age vs. Maximum Heart Rate
📌 Bar Chart: Heart disease comparison
📌 3D Plot: Age, Cholesterol, and Heart Disease
📌 Pie Chart: Chest Pain Type distribution
------------------------------------------------------------------------------------------------------------------------------
Initial Findings:
- The dataset contains 1025 rows and 14 columns.
- There are some missing values in the restecg and oldpeak columns.
- The dataset includes numerical features such as age, cholesterol (chol), blood pressure (trestbps), and heart rate (thalach).
- The target column indicates whether a patient has heart disease (1) or not (0).
Next Steps:
1- Handle missing values using mean imputation.
2- Display null value counts before and after imputation.
3- Detect and remove outliers for at least one column.
4- Perform numerical analysis (mean, median, standard deviation, etc.).
5- Visualize data using histograms, scatter plots, bar charts, pie charts, and 3D plots.
-------------------------------------------------------------------------------------------------------------------------------
Missing Value Handling:
* Before imputation: restecg had 1 missing value, and oldpeak had 2 missing values.
* After imputation: No missing values remain (all missing values were filled with the column mean).
  
Outlier Removal:
* Before removal: The dataset had 1025 rows.
* After removing cholesterol outliers: The dataset now has 1009 rows.
- This means 16 outliers were detected and removed.
------------------------------------------------------------------------------------------------------------------------------
Sorting & Searching Results:
1-Top 5 patients with highest cholesterol:
* Maximum cholesterol recorded: 360 mg/dL (age: 65).
* Second highest: 354 mg/dL (age: 57).
2- Patients with cholesterol above 300 mg/dL: 130 patients.

3- Patients older than 60 with abnormal ECG (restecg > 0): 120 patients.
-----------------------------------------------------------------------------------------------------------------------------
Reshaping & Splitting:
.The dataset was reshaped into a (1009, 14) array.
.It was split into three parts:
  - First part: 336 rows
  - Second part: 336 rows
  - Third part: 337 rows (slightly larger due to uneven division)
