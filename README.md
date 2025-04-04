# Bayesian Network for Diabetes Risk Analysis

This repository hosts the capstone project for the **Master of Science in Applied Data Science** at the **University of Chicago**, titled **“Causation Inference with Probabilistic Models”**. Our team applies Bayesian Networks to analyze health risk factors associated with diabetes, compare causal inference approaches, and provide interpretable insights for healthcare applications.

---

## 🎯 Project Overview

- **Goal**: To understand causal relationships between lifestyle, demographic, and health indicators related to diabetes using Bayesian Networks.
- **Approach**: Apply structure learning algorithms and causal inference techniques on CDC survey data, leveraging both domain knowledge and data-driven modeling.
- **Outcome**: A probabilistic model built using **AgenaRisk** and Python that enables causal reasoning and supports medical decision-making.

---

## 👩‍💻 Team

- **Zihao Liu**, **Siyu Han**, **Chao Tang**, **Yi Zhou**
- **Capstone Advisor**: Prof. Don Patchell, Dr. Yuri G. Balasanov, Founder & President, iLykei Teaching Tech Corp

---

## 📊 Datasets

### 1. **FemSmoke Dataset**
A teaching dataset with 28 observations showing relationships between age, smoking status, and death. Used for demonstrating causal inference and Simpson’s Paradox.

### 2. **Diabetes_012 Dataset**
Survey data from CDC’s BRFSS 2015 with 253,680 observations and 21 features related to health, lifestyle, and demographics. Used for building and evaluating the Bayesian model.

---

## 🧠 Methodology

- **Structure Learning Algorithms**:
  - Hill-Climbing Search (selected for final model)
  - Chow-Liu Tree
  - Tree-Augmented Naive Bayes (TAN)
  - Parameter Constraints

- **Modeling Tool**: [AgenaRisk](https://www.agenarisk.com/)
- **Causal Inference Concepts**:
  - Directed Acyclic Graphs (DAG)
  - Mutilation & Monte Carlo Simulations
  - Average Treatment Effect (ATE)
  - Simpson’s Paradox

- **Software**: Python (pgmpy, pandas), R, AgenaRisk

---

## ⚖️ Comparison with Multinomial Logistic Regression

| Aspect                        | Bayesian Network                             | Multinomial Logistic Regression              |
|------------------------------|----------------------------------------------|----------------------------------------------|
| **Causal Discovery**         | ✅ Supports causal inference with DAGs        | ❌ Limited to association                    |
| **Interpretability**         | ✅ Graphical + probabilistic reasoning         | ⚠️ Coefficient-based, but harder to interpret |
| **Handles Confounders**      | ✅ Visual + algorithmic control               | ❌ Requires manual selection                  |
| **Missing Data**             | ✅ Naturally handles                          | ❌ Requires imputation                        |
| **Use Case Fit**             | ✅ Diagnostics & decision-making              | ⚠️ Prediction-focused                        |

> In our study, logistic regression showed minor variations in risk prediction, while the Bayesian Network allowed us to visually and quantitatively trace how each factor contributed to diabetes, revealing deeper insight into variable interdependencies.

---

## 📈 Key Results

- The **Hill-Climbing Search algorithm** yielded the best-performing Bayesian Network with 86.05% accuracy.
- **Simpson’s Paradox** uncovered in the FemSmoke dataset: smokers appeared healthier until age was controlled for.
- **Causal effect (ATE)** of diabetes on heart disease estimated at **+10.6%**, supporting early lifestyle interventions.

---

## 🧪 Application Scenarios

In our **AgenaRisk demo**, we simulated clinical consultations:
- Predicted a patient's risk given lifestyle changes
- Evaluated treatment recommendations
- Showed visual outcomes with what-if analyses

---

## 📁 Repository Structure


