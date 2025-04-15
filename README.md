# 🏀 NBA Trends: Data Analysis Project

![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)
![Matplotlib](https://img.shields.io/badge/Library-matplotlib-orange)
![Seaborn](https://img.shields.io/badge/Library-seaborn-blue)
![License](https://img.shields.io/badge/License-MIT-green.svg)

This project analyzes NBA game data to uncover associations between game outcomes, team performance, and predictive probabilities. Using historical NBA data originally published by [FiveThirtyEight](https://github.com/fivethirtyeight/data/tree/master/nba-elo), we focus on select teams and seasons to perform exploratory data analysis and hypothesis testing.

---

## 📁 Dataset Overview

- Source: [FiveThirtyEight NBA Elo Data](https://github.com/fivethirtyeight/data/tree/master/nba-elo)
- Includes historical NBA game data from [Basketball Reference](https://www.basketball-reference.com/)
- Subset: Focused on 5 teams, 10 columns + 1 constructed column `point_diff`

**Constructed Column:**
- `point_diff`: The difference between a team’s score (`pts`) and opponent’s score (`opp_pts`)

---

## ✅ Objectives

- Analyze quantitative and categorical relationships in NBA data
- Visualize trends and differences between teams/seasons
- Evaluate predictive value of win probabilities
- Conduct hypothesis testing (e.g., chi-square test, correlation)

---

## 🧪 Key Analytical Steps

### 🔢 Comparing Team Performance (2010 vs. 2014)
- Calculated average point differences between Knicks and Nets for both 2010 and 2014
- Visualized score distributions using overlapping histograms
- Observed how mean differences changed over time

### 📊 Franchise vs. Points Scored
- Created side-by-side boxplots for each franchise’s point distributions
- Identified teams with significantly different scoring patterns

### 🏠 Home vs. Away Wins (Categorical Association)
- Created contingency tables for game result vs. location
- Converted counts to proportions
- Performed chi-square test to determine statistical association

### 📈 Forecast vs. Victory Margin (Quantitative Association)
- Calculated covariance and correlation between win probability (`forecast`) and score margin (`point_diff`)
- Generated scatter plot to visualize relationship
- Found a **moderate positive correlation** (r ≈ 0.44, p < 0.001)

---

## 📉 Key Functions Used

```python
# Covariance & Correlation
np.cov(), pearsonr()

# Frequency Tables
pd.crosstab()

# Visualization
plt.hist(), sns.boxplot(), plt.scatter()
```

---

## 📊 Visualizations
- 📉 Overlapping Histograms (Knicks vs. Nets, 2010 & 2014)
- 📦 Boxplots of Points by Franchise
- 🧮 Contingency Table for Home/Away Wins
- 📈 Scatter Plot: Forecasted Probability vs. Actual Margin

---

## 🛠 Tools Used

- Python 3
- pandas
- numpy
- matplotlib
- seaborn
- scipy.stats (for chi-square and correlation)

---

## 📁 Repository Structure
```
NBA-Trends-Analysis/
├── nba_games.csv
├── nba_trends_analysis.ipynb
├── README.md
```

---

## 📬 Contact

**Irmak Erkol**  
📧 irmakerkol00@gmail.com  
💼 [LinkedIn](https://linkedin.com/in/irmakerkol)

---

## 🌐 Project Link

[🔗 Codecademy NBA Trends Project](https://www.codecademy.com/projects/practice/nba-trends)

