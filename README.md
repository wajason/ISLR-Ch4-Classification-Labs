# 📈 ISLR Chapter 4.7: Classification Methods Lab Implementation

[![GitHub Stars](https://img.shields.io/github/stars/wajason/ISLR-Ch4-Classification-Labs?style=for-the-badge&logo=github&color=6699CC)](https://github.com/wajason/ISLR-Ch4-Classification-Labs/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/wajason/ISLR-Ch4-Classification-Labs?style=for-the-badge&logo=github&color=6699CC)](https://github.com/wajason/ISLR-Ch4-Classification-Labs/network/members)
[![Issues](https://img.shields.io/github/issues/wajason/ISLR-Ch4-Classification-Labs?style=for-the-badge&color=6699CC)](https://github.com/wajason/ISLR-Ch4-Classification-Labs/issues)
[![License](https://img.shields.io/badge/License-MIT-6699CC?style=for-the-badge)](./LICENSE)

This repository contains a comprehensive implementation and detailed annotation of the R code presented in Chapter 4.7 (Classification Methods) of *An Introduction to Statistical Learning* (James et al., 2021).

The aim is to provide a clear, step-by-step tutorial on applying various classification models to real-world datasets, complete with statistical rationale and model performance comparison.

---

## ✨ Key Features & Highlights

This tutorial goes beyond simply repeating the code by including:

* **Model Performance Comparison:** Directly compares the accuracy and predictive power of **Logistic Regression (GLM)**, **Linear Discriminant Analysis (LDA)**, **Quadratic Discriminant Analysis (QDA)**, **Naive Bayes**, and **K-Nearest Neighbors (KNN)** on the challenging S&P 500 (`Smarket`) dataset.
* **Best Model Identification:** QDA and Naive Bayes show significantly better performance on the `Smarket` data, achieving nearly 60% accuracy.
* **Handling Imbalanced Data:** Implementation and analysis of the `Caravan` insurance dataset, focusing on the true success rate (precision) rather than overall accuracy, highlighting the use of a modified prediction threshold (e.g., $P > 0.25$).
* **Count Data Modeling:** Includes the dedicated Section 4.7.7 on using **Poisson Regression** to model bike rental counts (`Bikeshare` dataset), visually demonstrating why the Linear Model fails to predict non-negative counts and extreme values.
* **Detailed Annotations:** Every line of R code is annotated with explanations of the underlying statistical theory and practical interpretation.

---

## 📂 Repository Structure

| File | Description |
| :--- | :--- |
| `Classification_Methods_Tutorials.pdf` | **The fully rendered tutorial.** Contains all R code, output, figures, and detailed personal commentary/analysis. |
| `README.md` | Project overview, links, and reproduction instructions. |

---

## 🛠️ Data Source & Reproduction

### Data Source
All data and primary code structure are derived from:
* **Book:** *An Introduction to Statistical Learning with Applications in R* (ISLR).
* **Authors:** Gareth James, Daniela Witten, Trevor Hastie, Robert Tibshirani (2021).
* **Packages:** Primarily relies on `ISLR2`, `MASS` (for LDA/QDA), `e1071` (for Naive Bayes), and `class` (for KNN).

### How to Reproduce
To recreate the analysis and figures locally:

1.  **Download** the PDF file to see the full code.
2.  Install the required R packages: `install.packages(c("ISLR2", "MASS", "e1071", "class"))`
3.  Copy the code from the PDF into an R environment and execute.
