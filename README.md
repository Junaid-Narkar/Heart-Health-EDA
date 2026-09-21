# Heart Health EDA

Exploratory Data Analysis on a heart disease dataset (303 patient records, 14 clinical features) to identify patterns and risk factors associated with heart disease diagnosis.

## Project Overview

This project performs a full exploratory data analysis on the UCI Heart Disease dataset. The goal is to understand how clinical measurements (age, cholesterol, chest pain type, resting blood pressure, etc.) relate to the presence of heart disease. The analysis is EDA-only — no machine learning models.

## Dataset

| Column | Description |
|---|---|
| age | Age in years |
| sex | 1 = female, 0 = male |
| cp | Chest pain type (0–3) |
| trestbps | Resting blood pressure (mm Hg) |
| chol | Serum cholesterol (mg/dl) |
| fbs | Fasting blood sugar > 120 mg/dl (1 = true, 0 = false) |
| restecg | Resting electrocardiographic results (0–2) |
| thalach | Maximum heart rate achieved |
| exang | Exercise induced angina (1 = yes, 0 = no) |
| oldpeak | ST depression induced by exercise |
| slope | Slope of peak exercise ST segment |
| ca | Number of major vessels colored by fluoroscopy (0–3) |
| thal | Thalassemia (1 = normal, 2 = fixed defect, 3 = reversible defect) |
| target | 1 = heart disease, 0 = no heart disease |

- Rows: 303
- Columns: 14
- Missing values: 0

## Tools Used

- Python 3
- pandas, numpy
- matplotlib, seaborn
- AutoViz, Sweetviz (automated EDA reports)
- Jupyter / Google Colab

## Analysis Steps

1. Loaded dataset and inspected structure with `df.info()` and `df.head()`
2. Plotted age distribution histogram
3. Plotted density plot of age by sex
4. Plotted resting blood pressure distribution and density
5. Boxplots for cholesterol and oldpeak
6. Countplots for all categorical features against target
7. Correlation heatmap of all numerical features
8. Scatterplot of cholesterol vs resting blood pressure by sex
9. Generated AutoViz and Sweetviz automated reports

## Key Insights

- Target distribution: 165 positive (heart disease), 138 negative
- No missing values in the dataset
- No feature pair shows strong correlation (above |0.7|)
- Age distribution: peak concentration between 57 and 63 years
- Resting blood pressure: approximately normal distribution
- Healthy males outnumber unhealthy males; unhealthy females outnumber healthy females
- Higher heart disease diagnosis rate among patients with chest pain
- Restecg ST-T wave abnormality → higher diagnosis rate
- Slope = 2 → higher diagnosis rate
- Thal = 2 → higher diagnosis rate
- Ca between 1 and 3 → diagnosis ratio decreases

## How to Run

1. Clone the repo:

git clone https://github.com/Junaid-Narkar/Heart-Health-EDA.git

2. Open the notebook `Heart-Health-EDA.ipynb` in Jupyter or Google Colab
3. Install dependencies:
4. Update the CSV path in the notebook to point to `heart-1.csv`
5. Run all cells

## Repository Structure

Heart-Health-EDA/
├── Heart-Health-EDA.ipynb
├── heart-1.csv
├── README.md
├── LICENSE
└── .gitignore

## Author

**Junaid Narkar**
Data Analyst | SQL · Power BI · Python
Kuwait
- LinkedIn: https://www.linkedin.com/in/junaidnarkar-analyst/
- GitHub: https://github.com/Junaid-Narkar