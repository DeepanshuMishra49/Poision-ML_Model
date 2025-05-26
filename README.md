# Poisoning a Machine Learning Model  
**Final Year Project | KIET Group of Institutions, Ghaziabad**

##  Project Overview
This project explores how **label poisoning attacks**—a form of adversarial attack—can degrade the performance of supervised machine learning models. We simulate label-flipping attacks across multiple datasets to assess the **robustness and vulnerability** of widely used classifiers like **SVM, Logistic Regression, Random Forest, and Decision Tree**.

---

##  Datasets Used
We conducted experiments on five real-world datasets from various domains:

1. **Heart Attack Dataset** – Predicts risk of heart attack from clinical features.
2. **Diabetes Dataset** – Predicts diabetes using medical parameters.
3. **Banking Dataset** – Customer data to predict term deposit subscription.
4. **Email (Spam) Dataset** – Classifies emails as spam or not based on content.
5. **Iris Dataset** – Multiclass classification of iris flower species.

---

##  Tech Stack & Dependencies

###  Programming Language
- Python 3.6+

###  Libraries Used
- `pandas` – Data handling  
- `numpy` – Numerical operations  
- `scikit-learn` – Model training, preprocessing, evaluation  
- `matplotlib`, `seaborn` – Data visualization  
- `random` – Simulating label poisoning  

To install dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
