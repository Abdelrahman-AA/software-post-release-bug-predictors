# 📘 software-post-release-bug-predictors
**Analysis of Some Factors Affecting Post-Release Number of Bugs in Software Applications**
_Statistical analysis of software metrics and their impact on the number of post-release bugs across 51 real-world Android applications._

![Made with SPSS](https://img.shields.io/badge/Made%20With-SPSS-blueviolet?style=flat-square)
![Statistics Project](https://img.shields.io/badge/Type-Statistics%20Study-green?style=flat-square)
![Open Source Dataset](https://img.shields.io/badge/Data-Open%20Source-orange?style=flat-square)

---

## 📊 Overview

This study explores the impact of key software metrics on the number of bugs discovered after releasing software applications. The goal is to understand which aspects of software development and testing contribute most to post-release bugs — and thus, how to improve software quality proactively.

The research relies on a dataset collected from 51 real-world open-source Android applications, analyzing factors such as lines of code, code complexity, testing duration, and coverage to understand their relationships with the number of post-release bugs.

---

## 🎯 Objectives

- Identify which software development metrics correlate most with post-release bugs.
- Quantify the strength and direction of these relationships using **correlation** and **regression analysis**.
- Suggest actionable improvements to software testing and quality assurance practices.

---

## 🔬 Variables

### 🎯 Dependent Variable
- **Post-Release Number of Bugs**: Bugs reported after application release.

### ⚙️ Independent Variables
- **Active Lines of Code (LOC)**
- **General Code Complexity (MI)**
- **Halstead Time (min)**
- **Automation Testing Hours**
- **Code Coverage (%)**
- **Number of Test Cases**

---

## 📈 Key Results

### 📉 Correlation Insights
- **Test Cases (r = 0.843)** and **Code Coverage (r = 0.762)** had the strongest positive correlations with post-release bugs.
- **Halstead Time** and **Automation Testing Hours** had moderate correlations.
- **Halstead Time** and **Automation Testing Hours** showed **moderate correlations**.
- **Active LOC** and **Code Complexity** had **weaker but statistically significant** correlations.

### 🧮 Regression Modeling
- **Test Cases alone** explained up to **71.1%** of bug variation.
- **All factors combined** explained **82%** of bug variation.
- The regression formula from the final model (All Variables) is:
```
Post-Release Bugs = 
-90.87 
+ (0.003 × LOC) 
- (2.871 × MI) 
+ (0.041 × AutoTestHours) 
+ (125.697 × Coverage) 
+ (0.035 × TestCases) 
+ ε
```

---

## 📂 Dataset Highlights

| App Name          | Bugs | LOC   | MI   | Halstead | Auto Test Hrs | Coverage | Test Cases |
|------------------|------|-------|------|----------|----------------|----------|------------|
| Signal           | 53   | 12480 | 20.5 | 69.3     | 312            | 74%      | 1239       |
| Telegram         | 82   | 16900 | 23.4 | 91.2     | 388            | 84%      | 1484       |
| Firefox          | 103  | 14200 | 22.1 | 102.3    | 341            | 81%      | 1183       |
| ...              | ...  | ...   | ...  | ...      | ...            | ...      | ...        |

Full dataset available in the PDF report.

---

## 🧾 Methodology

- **Tools used**: IBM SPSS, Excel
- **Statistical Methods**: Descriptive statistics, Pearson correlations, linear and multiple regression
- **Sample Size**: 51 Android apps from open-source platforms
- **Data Range**: Varies across metrics like LOC (3k–24k), Test Cases (300–2300), Coverage (52%–90%)

---

## 📄 View Full Report

You can view the full report from the link below:

🔗 [View full Report](https://github.com/Abdelrahman-AA/software-post-release-bug-predictors/blob/main/Analysis%20of%20some%20Factors%20Affecting%20Post-Release%20Number%20of%20Bugs%20in%20Software%20Applications.pdf)

---

## 🧑‍💻 Study Author

**Abdelrahman Abodief Mohamed**

---

## 📘 Suggested Improvements for Development Teams

Based on this analysis, teams can reduce post-release bugs by:

- Investing more in writing **effective test cases**
- Increasing **automated test coverage**
- Refactoring to reduce **code complexity**
- Monitoring and optimizing **testing time allocation**
- Focusing on code quality metrics early in the development lifecycle

---

## 📌 License

This project is shared **strictly for educational purposes only**.

- Reuse or redistribution of any part of this project is **prohibited** without **explicit written permission** from the author.
- Attribution **must** be provided as:  
**"Abdelrahman Abodief Mohamed – Author of the study on post-release bug analysis"**
- **Commercial use is not allowed.**

---
