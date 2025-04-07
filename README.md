# 📊 Machine Learning with R: A Practical Guide

This repository presents a hands-on walkthrough of machine learning using R, with a focus on explainable AI and real-world application. R is a powerful language for statistical computing, and with its extensive ecosystem of packages, it provides an accessible platform for machine learning and data mining.

In this guide, we explore the **Boston Housing dataset** to demonstrate how to:
- Apply the **CRISP-DM** (Cross-Industry Standard Process for Data Mining) methodology,
- Perform **feature selection** using explainable AI tools, and
- Derive actionable business insights from a trained model.

---

## 🧭 CRISP-DM Process

The CRISP-DM framework provides a structured approach to data science projects. While the full process includes six phases, this tutorial focuses on the core technical stages:

1. **Business Understanding**  
2. **Data Understanding** ✅  
3. **Data Preparation** ✅  
4. **Modeling** ✅  
5. **Evaluation** ✅  
6. Deployment *(out of scope for this tutorial)*

---

## 🔍 Data Understanding

We begin with exploratory data analysis to understand the structure, distribution, and key variables of the dataset. The `summary()` function in R provides a quick statistical overview.

Our **target variable** is `medv` — the median value of owner-occupied homes (in $1000s). Understanding the distributions and relationships among variables helps inform subsequent preprocessing and modeling decisions.

```r
# Load dataset
library(MASS)
data("Boston")

# View summary statistics
summary(Boston)
