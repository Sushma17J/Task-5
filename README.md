# 📝 Titanic Dataset – Exploratory Data Analysis (EDA)

This project explores the "Titanic survival dataset" using Python to uncover key insights about passenger demographics, travel classes, and survival patterns.

---

## 📊 Analysis Steps
1. **Import & Load Data**  
   - Libraries: `pandas`, `seaborn`, `matplotlib`  
   - Load `train.csv` and inspect first few rows.

2. **Basic Info & Summary Stats**  
   - Dataset shape, data types, and descriptive statistics.
   - Check categorical value counts for `Sex`, `Pclass`, `Embarked`.

3. **Missing Value Analysis**  
   - Heatmap to visualize missingness.
   - Observations:
     - `Cabin` → Many missing values.
     - `Age` → ~177 missing.
     - `Embarked` → 2 missing.

4. **Univariate Analysis**  
   - **Numerical:** Histograms & boxplots for `Age` and `Fare`.
   - **Categorical:** Bar charts for `Sex`, `Pclass`, `Embarked`.
   - Key findings:
     - Age is slightly right-skewed (most passengers 20–40 years).
     - Fare is heavily right-skewed with outliers.
     - More males than females; most passengers are 3rd class.

5. **Bivariate Analysis**  
   - Survival rate by `Sex`, `Pclass`, `Embarked`.
   - Age vs Survival (stacked histograms).
   - Fare vs Survival (boxplots).
   - Key findings:
     - Females had a much higher survival rate.
     - 1st class passengers survived the most; 3rd class the least.
     - Children had higher survival; higher fares correlate with survival.

6. **Correlation Analysis**  
   - Heatmap of numeric correlations.
   - Strong negative correlation: `Pclass` vs `Survived`.
   - Positive correlation: `Fare` vs `Survived`.

7. **Optional Pairplot**  
   - Quick multivariate overview of relationships.
