# Mental Health and Social Media Balance Analysis

![Project Banner](image1.jpg)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python Version](https://img.shields.io/badge/Python-3.13-blue.svg)](https://www.python.org/downloads/release/python-3130/)

This repository contains a **data analysis project** exploring how **social media usage**, **screen time**, and **lifestyle habits** affect **mental health indicators** such as happiness, stress, and sleep quality.

The project uses a **dataset of 500 users** and a **Jupyter Notebook** to perform descriptive statistics, EDA, ML modeling, and visualization.

---

## Project Overview
Social media has become an integral part of modern life, but its impact on well‑being is widely debated. This project analyzes user demographics, platform preferences, and daily habits to uncover patterns affecting mental health.

### Tools used
- **Pandas**, **NumPy** – data preparation
- **Matplotlib**, **Seaborn**, **Plotly** – visualization
- **Scikit-Learn** – modeling (Random Forest)
- **Optuna** – hyperparameter tuning
- **Feature-engine**, **SciPy** – transformations and statistical analysis

**Key components:**
- Dataset: `Mental_Health_and_Social_Media_Balance_Dataset.csv`
- Notebook: `da_social_media_stress.ipynb`
- Model: Random Forest Regressor
- Visualization: Interactive probability cloud

---

## Objectives
- Analyze the impact of screen time on stress, sleep, and happiness
- Evaluate lifestyle factors (exercise, social media‑free days)
- Compare mental health across age groups, gender, and platforms
- Study correlations and develop a predictive model

---

## Dataset
**File:** Mental_Health_and_Social_Media_Balance_Dataset.csv  
**Source:** Kaggle  
**Size:** 500 rows

| Column | Description |
|--------|-------------|
| User_ID | Unique identifier |
| Age | 16–49 years |
| Gender | Male, Female, Other |
| Daily_Screen_Time(hrs) | Average daily screen time |
| Sleep_Quality(1-10) | Self‑reported sleep quality |
| Stress_Level(1-10) | Self‑reported stress |
| Days_Without_Social_Media | Days per week not using social media |
| Exercise_Frequency(week) | Weekly exercise frequency |
| Social_Media_Platform | Main platform used |
| Happiness_Index(1-10) | Self‑reported happiness |

---

## Key Findings
![Correlation Heatmap](correlation_heatmap.png)

- Low screen time + regular exercise yields the **highest happiness**
- **Instagram** users show **lower average happiness**
- Sleep quality strongly predicts both happiness and stress
- Stress levels are similar across demographics

---

## Requirements
Use the included `requirements.txt` for installation:
```
pip install -r requirements.txt
```
Or manually install:
```
pandas
numpy
matplotlib
seaborn
plotly
scikit-learn
optuna
feature-engine
scipy
```

---

## How to Reproduce
### **1. Clone the repository**
```bash
git clone https://github.com/your-username/mental-health-social-media-analysis.git
cd mental-health-social-media-analysis
```

### **2. Set up the environment**
**Linux/macOS:**
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

**Windows:**
```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

### **3. Run the notebook**
```bash
jupyter notebook
```
Open `da_social_media_stress.ipynb` → **Restart & Run All**.

### **4. Make predictions**
Modify the example user in the notebook:
```python
new_user = pd.DataFrame([{
    "Age": 27,
    "Daily_Screen_Time(hrs)": 4.2,
    "Social_Media_Platform": "Instagram",
    "Exercise_Frequency(week)": 4,
    "Days_Without_Social_Media": 1,
    "Sleep_Quality(1-10)": 6
}])
```
Re-run the prediction cells to generate a new probability cloud.

---

## Contributing
Please follow best practices:
- Fork the repository
- Create a feature branch
- Commit with clear messages
- Open a Pull Request

If you plan to contribute regularly, consider adding:
- `CONTRIBUTING.md`
- `CODE_OF_CONDUCT.md`

---

## License
This project is licensed under the **MIT License**.

---

## Author
**Volodymyr Babunych**  
📧 vbabunych@gmail.com  
📍 United Kingdom  
🗓️ November 11, 2025
