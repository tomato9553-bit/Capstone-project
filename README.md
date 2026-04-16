# Capstone Mini Project - NHANES 2020 Body Measurement Analysis

A data analysis project exploring body measurements from the **National Health and Nutrition Examination Survey (NHANES) 2020** dataset using NumPy, Matplotlib, SciPy, and Seaborn.

---

## Overview

This notebook compares body measurements between adult males and females and evaluates three common adiposity metrics: **BMI**, **waist-to-height ratio (WHtR)**, and **waist-to-hip ratio (WHR)**. The entire analysis is built on NumPy matrix operations without relying on high-level dataframe abstractions, making it a practical exercise in numerical computing.

---

## Dataset

- **Source:** [gagolews/teaching-data](https://github.com/gagolews/teaching-data) (NHANES Adult BMX 2020)
- **Files:** `nhanes_adult_male_bmx_2020.csv` and `nhanes_adult_female_bmx_2020.csv`
- **Columns (7):** Weight, Standing Height, Upper Arm Length, Upper Leg Length, Arm Circumference, Hip Circumference, Waist Circumference

> Data is loaded directly from GitHub using `np.genfromtxt`. Rows with missing values are removed prior to analysis.

---

## Project Structure

```
Capstone_mini_project.ipynb   # Main analysis notebook
README.md
```

---

## Analysis Sections

| Section | Description |
|---------|-------------|
| 1 | Importing libraries and loading data |
| 2 | Histograms of male and female weight distributions |
| 3 | Box-and-whisker plot comparing weights by sex |
| 4 | Descriptive statistics (mean, median, std, IQR, skewness, kurtosis) |
| 5 | Computing and appending the BMI column |
| 6 | Z-score standardisation of the female dataset |
| 7 | Pairplot matrix and Pearson/Spearman correlation analysis |
| 8 | Adding WHtR and WHR columns to both matrices |
| 9 | Boxplot comparing WHtR and WHR across sexes |
| 10 | Advantages and disadvantages of BMI, WHtR, and WHR |
| 11 | Identifying extreme BMI participants (lowest/highest 5) |

---

## Key Findings

  Certainly! Here’s a more readable and copy-friendly reformatted **Key Findings** section. You can copy and paste this directly into your README.

---

## Key Findings

- **Males were heavier on average**
  - Greater variability in weight compared to females.
- **Both distributions are right-skewed**
  - Most participants fall in lower weight ranges, with a tail of high values.
- **Weight and BMI are strongly correlated**
  - Correlation coefficient: ~0.9+ (Pearson), as expected from the BMI formula.
- **Males had substantially higher WHR than females**
  - Consistent with known patterns of abdominal fat distribution.
- **Height showed weak correlation with waist and hip circumference**
  - Suggests height is a poor predictor of body composition in this dataset.
- **Highest-BMI individuals profile**
  - Scored well above average on all circumference measures.
  - At or below average in height.

---

Feel free to adjust the wording as needed for your audience!

---

## Tech Stack

- **Python 3**
- [NumPy](https://numpy.org/) - matrix operations and numerical computing
- [Matplotlib](https://matplotlib.org/) - histograms and boxplots
- [SciPy](https://scipy.org/) - skewness, kurtosis, and correlation tests
- [Seaborn](https://seaborn.pydata.org/) - pairplot matrix
- [Pandas](https://pandas.pydata.org/) - DataFrame wrapper for pairplot only

---

## How to Run

1. Clone this repository
2. Install dependencies:
   ```bash
   pip install numpy matplotlib scipy seaborn pandas
   ```
3. Open the notebook:
   ```bash
   jupyter notebook Capstone_mini_project.ipynb
   ```

> An active internet connection is required - the CSV files are loaded directly from GitHub.

---

## Limitations

- Missing rows are dropped entirely rather than imputed; a more rigorous approach would investigate the pattern of missingness.
- The dataset covers US adults in 2020 only, so findings may not generalise to other populations or time periods.
- Waist and hip measurements can vary depending on measurement technique, which may affect the reliability of ratio-based metrics.

---

## Author

**M. Gopal** | Data Science  
*Initiated: 08-04-2026 | Completed: 15-04-2026*
