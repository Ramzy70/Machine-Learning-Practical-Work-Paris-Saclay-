# M2 AI & Machine Vision: Machine Learning Practicle Work

This repository contains a collection of core machine learning algorithms implemented during my M2 at **Université Paris-Saclay**. The focus of these projects is "from-scratch" implementation using **NumPy** to deeply understand the underlying mathematics and optimization techniques required for research in AI and Computer Vision.

---

## 🚀 Projects Overview

### 1. Robust Linear Regression & Estimation
* **Source:** `tp1.ipynb`
* **Objective:** Implementing and comparing various regression techniques on datasets with significant noise and outliers.
* **Key Implementations:**
    * **Ordinary Least Squares (OLS):** Closed-form solution using the Normal Equation.
    * **L2 Regularization (Ridge):** Analysis of how $\lambda$ affects coefficient variance and model complexity.
    * **RANSAC (Random Sample Consensus):** An iterative method to estimate parameters of a mathematical model from a set of observed data that contains outliers.
* **Research Insight:** Demonstrated the breakdown point of OLS and why RANSAC is the gold standard for robust fitting in computer vision tasks.

### 2. Decision Tree Classifier from Scratch
* **Source:** `tp2.ipynb`
* **Objective:** Building a recursive partitioning model for non-linear classification without high-level libraries.
* **Key Implementations:**
    * **Recursive Tree Construction:** Implementing the greedy top-down approach for splitting data.
    * **Impurity Metrics:** Implementation of **Gini Impurity** and **Information Gain** to determine the best feature-split pairs.
    * **Visualization:** Integration with Graphviz (DOT format) to visualize the decision logic and tree depth.

### 3. Dimensionality Reduction & Adam Optimization
* **Source:** `course 3.ipynb`
* **Objective:** Solving high-dimensional regression problems using custom-built optimization loops.
* **Key Implementations:**
    * **Dimensionality Reduction:** Reducing feature space (PCA-style) before model training to handle the "curse of dimensionality."
    * **Adam Optimizer:** A pure NumPy implementation of the **Adaptive Moment Estimation** algorithm, including first/second moment estimates and bias correction.
* **Critical Analysis:** Includes an evaluation of Mean Squared Error (MSE) vs. R-squared metrics, specifically discussing why linear models can sometimes yield negative R-squared values after aggressive dimensionality reduction.

---

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Core Libraries:** `NumPy` (Linear Algebra), `Matplotlib` (Visualization)
* **Scientific Tools:** `Scikit-Learn` (for benchmarking/comparison)
