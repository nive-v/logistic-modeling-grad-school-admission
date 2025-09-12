# Graduate School Admission Prediction  

This project applies **logistic regression (logit model)** to predict graduate school admissions based on applicants' academic performance and undergraduate institution prestige.  

---

## Problem Statement  
Logistic regression, also called a **logit model**, is used to model **dichotomous outcome variables**. In this project, the outcome variable is **admission**:  

- **1 = Admitted**  
- **0 = Not Admitted**  

The log odds of admission are modeled as a linear combination of the predictor variables.  

---

## Dataset  
The dataset used is **Graduate_School_Admission.csv**, which contains the following variables:  

- **admit** *(binary response variable)*:  
  - 1 = Admitted  
  - 0 = Not admitted  

- **GRE** *(continuous predictor)*: Graduate Record Exam scores  

- **GPA** *(continuous predictor)*: Grade Point Average  

- **rank** *(categorical predictor)*: Prestige of the undergraduate institution  
  - 1 = Highest prestige  
  - 4 = Lowest prestige  

---

## Objective  
The goal is to build a **logistic regression model** to analyze how **GRE scores, GPA, and institutional rank** influence graduate school admission decisions.  

---

## Steps Involved  
1. **Load and inspect the dataset**  
2. **Preprocess data**  
   - Handle categorical encoding for `rank`  
   - Standardize/normalize variables if necessary  
3. **Build the logistic regression model** using all predictors:  
   \[
   \text{logit}(p) = \beta_0 + \beta_1 \cdot GRE + \beta_2 \cdot GPA + \beta_3 \cdot rank
   \]  
4. **Interpret coefficients** to understand how each factor impacts admission chances  
5. **Evaluate the model** using metrics such as accuracy, precision, recall, and ROC-AUC  

---

## Tools & Libraries  
- Python 3  
- pandas  
- numpy  
- scikit-learn  
- statsmodels  
- matplotlib/seaborn

---

## Expected Outcome  
- A trained **logistic regression model**  
- Statistical interpretation of the effect of GRE, GPA, and rank on admission  
- Insights into how academic and institutional factors influence graduate school admission decisions  

---

## File Structure  
- Graduate_School_Admission.csv # Dataset
- Logistic_Regression_Grad_School.ipynb # Model building & analysis notebook
- README.md

## Author  
Research project built as part of coursework on **Logistic Regression & Predictive Modeling**.  
