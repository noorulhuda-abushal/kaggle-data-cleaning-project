# 🎓 Student Performance Analysis

Cleaning and analyzing a Kaggle dataset to understand which factors affect students' final scores.

## 🎯 Goal
Find out what really drives student success: study habits, attendance, lifestyle, or past performance?

## 📊 Dataset
- **Source:** Kaggle — Student Performance dataset
- **Size:** 1,000 students × 18 features
- **Includes:** final score, grade, pass/fail, previous scores (math, science, language), study hours, attendance, homework rate, sleep, screen time, physical activity, motivation, exam anxiety, parent education, study environment

## 🛠 Tools
Python · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn

## 🔄 What I Did
1. **Data inspection:** checked structure, types, and statistics
2. **Data quality:** checked for missing values, duplicates, inconsistent labels, and invalid values
3. **Cleaning:**
   - Filled missing `grade` values based on `final_score`
   - Filled missing categorical values using the mode
   - No rows were removed, so all 1,000 records were kept
4. **EDA:** histograms, scatter plots, boxplots, and a correlation heatmap
5. **Outliers:** IQR method (only `sleep_hours` had a few outliers)
6. **Transformation:** StandardScaler for numbers, One-Hot Encoding for categories
7. **Feature engineering:** created `performance_level` (Low / Average / Good / Excellent)
8. **Feature selection & PCA:** correlation-based selection and dimensionality reduction

## 💡 Key Insights
- **Previous scores are the strongest predictor** of the final score (correlation ≈ 0.84)
- **Attendance matters a lot** (correlation ≈ 0.74)
- **Study hours and homework completion** have a moderate positive effect
- **Sleep, screen time, and physical activity** have little impact
- **93% of students passed**, and most scored in the average range (grades C–D)

**Conclusion:** academic history and consistent engagement matter much more than lifestyle factors.


## 📁 Files
- `final_project.ipynb`: full analysis notebook
