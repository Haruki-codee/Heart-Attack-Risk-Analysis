# Heart Attack Risk Analysis 🫀

A data analysis project that explores key risk factors associated with heart attacks using a structured patient dataset. The notebook covers data loading, cleaning, feature engineering, and visual analysis.


## 📊 Dataset

**File:** `heart_attack_prediction_dataset.csv`

**Features used in analysis:**

| Feature | Description |
|---|---|
| Age | Patient age |
| Sex | Gender (Male / Female) |
| Cholesterol | Cholesterol level |
| Blood Pressure | Systolic/Diastolic (split into two columns) |
| Heart Rate | Resting heart rate |
| Diabetes | Diabetic or not (Yes/No) |
| Family History | Family history of heart disease (Yes/No) |
| Smoking | Smoking habit (Yes/No) |
| Obesity | Obese or not (Yes/No) |
| Alcohol Consumption | Alcohol use (Yes/No) |
| Exercise Hours Per Week | Weekly exercise hours (rounded up) |
| Diet | Dietary habits |
| Previous Heart Problems | Prior cardiac issues (Yes/No) |
| Stress Level | Categorized as Normal / Moderate / Little High / Extreme |
| Sedentary Hours Per Day | Daily sedentary hours (rounded up) |
| Triglycerides | Categorized as Normal / Borderline / High / Very High |
| Physical Activity Days Per Week | Active days per week |
| Sleep Hours Per Day | Categorized as Light / Moderate / Healthy |
| Heart Attack Risk | Target variable (Yes/No) |

---

## 🔧 Data Preprocessing Steps

1. **Subset selection** — Extracted 19 relevant columns from the raw dataset
2. **Binary encoding** — Converted `0/1` flags to readable `Yes/No` labels for: Diabetes, Family History, Smoking, Obesity, Alcohol Consumption, Previous Heart Problems, Heart Attack Risk
3. **Blood Pressure split** — Parsed `Systolic/Diastolic` format into two separate numeric columns
4. **Sleep categorization** — Grouped sleep hours into: `Light` (1–4 hrs), `Moderate` (5–6 hrs), `Healthy` (7+ hrs)
5. **Triglycerides categorization** — Grouped into: `Normal` (<150), `Borderline` (150–199), `High` (200–499), `Very High` (500+)
6. **Stress level categorization** — Grouped stress scores (1–10) into: `Normal`, `Moderate`, `Little High`, `Extreme`
7. **Exercise & Sedentary hours** — Ceiled to nearest integer for cleaner grouping

---

## 📈 Visualizations (Completed)

- **Heart Attack Risk by Gender** — Pie chart showing male vs. female distribution among at-risk patients

---

## 🚧 Upcoming Work

- Distribution plots for Age, Cholesterol, Heart Rate
- Risk breakdown by lifestyle factors (Smoking, Obesity, Diet)
- Correlation heatmap
- Feature importance analysis
- Predictive model (Logistic Regression / Random Forest)

---

## 🛠️ Requirements

```
python >= 3.8
numpy
pandas
matplotlib
```

Install dependencies:

```bash
pip install numpy pandas matplotlib
```

---

## 🚀 How to Run

1. Clone the repository or download the files
2. Place `heart_attack_prediction_dataset.csv` in the same directory as the notebook
3. Open the notebook:

```bash
jupyter notebook Heart_Attack_Risk_Analysis.ipynb
```

4. Run all cells in order (`Kernel > Restart & Run All`)

---

## 👤 Author

> Add your name, GitHub profile, or contact info here.

---

## 📄 License

This project is for educational and analytical purposes.
