# Impact of Procrastination on the Academic Performance of University Students

A statistical research project examining whether academic procrastination affects the academic performance (GPA) of university students in Khyber Pakhtunkhwa (KPK), Pakistan.

---

## Overview

Academic procrastination—the tendency to delay or postpone academic tasks—is widely reported among university students and is often considered a potential factor influencing academic performance. This project investigates whether procrastination is associated with students' GPA using self-reported survey data collected from university students across Khyber Pakhtunkhwa (KPK), Pakistan through standard statistical hypothesis testing.

---

## Objective

To determine whether procrastination has a statistically significant impact on the academic performance (GPA) of university students and whether this relationship differs by gender or academic year.

---

## Data Collection

- **Method:** Online questionnaire distributed via Google Forms
- **Population:** University students across Khyber Pakhtunkhwa (KPK), Pakistan (not restricted to any single institution)
- **Sample Size:** 150 responses

### Variables Collected

#### Demographic Information
- Gender
- Age Group
- Field of Study
- Academic Year

#### Academic Performance
- GPA in the last semester (collected as ranges)

#### Procrastination Assessment
Ten Likert-scale statements (Strongly Agree → Strongly Disagree) measuring procrastination behaviors such as:
- Task delay
- Distraction
- Guilt
- Motivation
- Awareness of consequences

---

## Methodology

The analysis was conducted in **Python** using **pandas, NumPy, SciPy, matplotlib, and seaborn** through the following stages:

1. **Data Loading**
   - Import raw Google Forms responses (CSV)

2. **Data Cleaning & Preprocessing**
   - Check for missing values and duplicates
   - Remove unnecessary spaces from column names
   - Verify data types

3. **Data Encoding**
   - Convert Likert responses to numerical values (1 = Strongly Agree … 5 = Strongly Disagree)
   - Convert GPA ranges to numeric midpoints

4. **Descriptive Statistics**
   - Mean
   - Median
   - Mode
   - Variance
   - Standard Deviation
   - Range
   - Interquartile Range (IQR)
   - Frequency and percentage distributions

5. **Data Visualization**
   - Demographic bar charts
   - GPA distribution
   - Average score per questionnaire item
   - Histogram of average procrastination scores
   - Gender-based boxplots
   - Academic year boxplots
   - Correlation heatmap across all ten Likert items

6. **Inferential Statistics** *(α = 0.05)*
   - Independent Samples **t-test**
   - **Pearson Correlation**
   - **One-way ANOVA**

7. **Correlation and Regression Analysis**
   - Simple Linear Regression to evaluate whether GPA can be predicted from procrastination score

8. **Interpretation & Conclusion**
   - Interpretation of statistical findings
   - Discussion of limitations
   - Recommendations for future research

---

## Key Findings

### Descriptive Statistics

- **Average procrastination score:** 2.759 (between *Agree* and *Neutral*, indicating a moderate tendency to procrastinate)
- **Average GPA:** 3.197
- **Sample distribution:** 84 Male, 63 Female, 3 Prefer not to say

### Hypothesis Testing

| Test | Statistic | p-value | Result |
|------|----------:|--------:|--------|
| Independent Samples *t*-test | t = -0.284 | 0.777 | No statistically significant difference in procrastination between male and female students |
| Pearson Correlation | r = 0.169 | 0.039 | **Weak but statistically significant positive correlation between procrastination score and GPA** |
| One-way ANOVA | F = 1.342 | 0.257 | No statistically significant difference in procrastination across academic years |

### Regression Analysis

**Regression Equation**

```text
GPA = 2.7848 + (0.1493 × Procrastination Score)
```

- **R² = 0.0285**

This indicates that procrastination explains only **2.85%** of the variation in students' GPA.

---

## Conclusion

The analysis identified a **statistically significant but weak relationship** between procrastination score and academic performance. Although the relationship reached statistical significance, its practical effect was very small, with procrastination accounting for less than **3%** of the variation in GPA. This suggests that additional factors—such as study habits, attendance, course difficulty, learning strategies, and individual ability—are likely to play a much larger role in determining students' academic performance.

Furthermore, neither **gender** nor **academic year** showed a statistically significant association with procrastination levels within the surveyed sample.

---

## Limitations

- Self-reported survey responses may introduce response bias.
- GPA was collected as ranges rather than exact values, reducing measurement precision.
- Sample sizes across academic years were uneven, with relatively few responses from first- and fifth-year students.
- Findings may not generalize beyond the surveyed population.

---

## Suggested Improvements

- Collect exact GPA values rather than GPA ranges.
- Increase the sample size, particularly for underrepresented academic years.
- Include additional explanatory variables such as study hours, attendance, part-time employment, living arrangements, and extracurricular involvement.

---

## Tools & Libraries

- Python 3
- pandas
- NumPy
- SciPy
- matplotlib
- seaborn

---

## Project Files

| File | Description |
|------|-------------|
| **main_project.ipynb** | Complete Jupyter Notebook containing data preprocessing, descriptive statistics, visualizations, hypothesis testing, regression analysis, and conclusions. |
| **Form Responses.csv** | Raw survey responses collected through Google Forms. |
| **cleaned_Responses.csv** | Cleaned and encoded dataset used for statistical analysis. |

---

## Repository Structure

```text
.
├── main_project.ipynb
├── Form Responses.csv
├── cleaned_Responses.csv
└── README.md
```

---

## Author

**Malaika Jabeen**  
BS Computer Science Student  
Islamia College Peshawar

 **Email:** hanimalaika90@gmail.com

 **LinkedIn:** https://www.linkedin.com/in/malaika-jabeen-596a203ab

 **GitHub:** https://github.com/mjcodes-77

---

## License

This project is shared for **educational and research purposes**. Please provide appropriate attribution if you use or reference this work.