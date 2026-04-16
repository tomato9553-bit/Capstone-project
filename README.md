<details>
<summary>🧑‍🔬 Capstone Mini Project - NHANES 2020 Body Measurement Analysis</summary>

![Python](https://img.shields.io/badge/python-3.7%2B-blue?logo=python)
![License](https://img.shields.io/badge/license-MIT-brightgreen)
![Status](https://img.shields.io/badge/status-completed-success)
![Last Update](https://img.shields.io/badge/updated-April%202026-orange)

> **A data-driven exploration of adult body metrics from the National Health and Nutrition Examination Survey (NHANES) 2020.**

</details>

---

<details>
<summary>📊 Project Overview</summary>

This project analyses body measurements of US adults from the **NHANES 2020** survey, with a particular focus on comparing males and females across several body composition metrics:
- **BMI (Body Mass Index)**
- **Waist-to-Height Ratio (WHtR)**
- **Waist-to-Hip Ratio (WHR)**

Utilizes powerful Python tools: `NumPy`, `SciPy`, `Matplotlib`, `Seaborn`, and `Pandas`.

</details>

---

<details>
<summary>🗂️ Dataset</summary>

- **Source:** [gagolews/teaching-data](https://github.com/gagolews/teaching-data) (NHANES Adult BMX 2020)
- **Files:**  
  - `nhanes_adult_male_bmx_2020.csv`  
  - `nhanes_adult_female_bmx_2020.csv`
- **Columns:**  
  Weight | Height | Upper Arm/Leg Length | Arm/Hip/Waist Circumference

> ℹ️ Data loaded directly from GitHub with `np.genfromtxt`. Rows with missing values are dropped before analysis.

</details>

---

<details>
<summary>🧩 Project Structure</summary>

```plaintext
Capstone_mini_project.ipynb   # Main Jupyter analysis
README.md                     # This file
```

</details>

---

<details>
<summary>🧠 Analysis Workflow</summary>

| Section | Description                                             |
|---------|--------------------------------------------------------|
| 1       | Importing libraries and loading data                    |
| 2       | Histogram comparison: male vs. female weight           |
| 3       | Box-and-whisker: weights by sex                        |
| 4       | Descriptive statistics & distribution shape             |
| 5       | Computing BMI                                          |
| 6       | Z-score standardization (female dataset)               |
| 7       | Pairplot matrix + correlation analysis (Pearson/Spearman) |
| 8       | Calculating WHtR and WHR                               |
| 9       | Boxplots: WHtR & WHR by sex                            |
| 10      | Pros & cons of BMI, WHtR, WHR                          |
| 11      | Extreme BMI participants (lowest/highest 5)            |

</details>

---

<details>
<summary>✨ <strong>Key Findings (click to expand)</strong></summary>

- **Males were heavier on average**  
  Greater variability in weight compared to females.
- **Both distributions are right-skewed:**  
  Most participants fall in lower weight ranges, with a tail of high values.
- **Weight and BMI are strongly correlated:**  
  - Correlation coefficient ~0.9+ (Pearson).
- **Males had substantially higher WHR:**  
  - Consistent with abdominal fat distribution patterns.
- **Height weakly correlated with waist/hip circumference:**  
  - Height alone is a poor predictor of body composition here.
- **Highest BMI individuals:**  
  - Above average on all circumference measures; average or below for height.

</details>

---

<details>
<summary>⚙️ Tech Stack</summary>

- **Python 3.7+**
- [NumPy](https://numpy.org/) — numerical computing
- [Matplotlib](https://matplotlib.org/) — data visualization
- [SciPy](https://scipy.org/) — stats/correlation/skewness/kurtosis
- [Seaborn](https://seaborn.pydata.org/) — advanced pairplots
- [Pandas](https://pandas.pydata.org/) — used for DataFrame creation

</details>

---

<details>
<summary>How to start</summary>

1. **Clone this repo:**
   ```bash
   git clone https://github.com/tomato9553-bit/Capstone-project.git
   cd Capstone-project
   ```
2. **Install dependencies:**
   ```bash
   pip install numpy matplotlib scipy seaborn pandas
   ```
3. **Open the Jupyter notebook:**
   ```bash
   jupyter notebook Capstone_mini_project.ipynb
   ```

> 💡 _Requires an active internet connection to fetch the dataset._

</details>

---

<details>
<summary>⚠️ Limitations</summary>

- Missing rows are dropped (not imputed)
- Dataset limited to US adults (2020) — results may not generalize
- Measurement variability (waist/hip ratios) may affect reliability

</details>

---

<details>
<summary>⏳ Timeline</summary>

- **Initiated:** 08-04-2026  
- **Completed:** 15-04-2026  

</details>

---

<details>
<summary>👤 Author</summary>

**M. Gopal**  
_Data Science Enthusiast_

</details>

---

<details>
<summary>✅ Project Checklist</summary>

- [x] Data import/validation
- [x] Exploratory analysis
- [x] Metrics calculation (BMI, WHtR, WHR)
- [x] Visualization & stats
- [x] Summarize findings
- [x] Write-up complete

</details>

---

> _Have questions or suggestions? Open an issue or pull request!_
