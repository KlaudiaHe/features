# Porównanie modeli uczenia maszynowego w credit scoringu

---

Celem projektu jest analiza i porównanie różnych modeli uczenia maszynowego stosowanych w credit scoringu, ze szczególnym uwzględnieniem selekcji zmiennych i technik Explainable AI (XAI).  
W badaniu wykorzystano rzeczywiste dane kredytowe (Freddie Mac Single-Family Loan-Level Dataset).

### Modele
- **`Models.ipynb`** – modele:
  - regresja logistyczna (benchmark),  
  - sieć neuronowa (MLP),  
  - lasy losowe.  
- **`XGBoost code.ipynb`** – implementacja XGBoost z analizą XAI.  
- **`CatBoost code.ipynb`** – implementacja CatBoost z analizą XAI.  

### Zakres analizy
- Przygotowanie danych i tworzenie flagi default (`Data_preparation.ipynb`)  
- Budowa i trenowanie modeli ML  
- Ewaluacja skuteczności predykcyjnej (AUC, ROC, PRC, confusion matrix)  
- Selekcja i porównanie zmiennych między modelami  
- Analizy XAI: SHAP, PDP, analiza błędów, stabilność w czasie  

---

## Technologie
- Python (pandas, numpy, scikit-learn, matplotlib, seaborn)  
- XGBoost, CatBoost  
- SHAP, PDP  
- DuckDB (przygotowanie danych)  

---

## Wyniki
Analizy potwierdziły kluczową rolę zmiennych takich jak:  
`credit_score`, `interest_rate`, `dti`, `first_payment_year` – które konsekwentnie zajmowały wysokie pozycje w rankingach ważności, niezależnie od algorytmu.  

---

# Comparison of Machine Learning Models in Credit Scoring
---

## Project Description
The goal of this project is to analyze and compare machine learning models applied to credit scoring, with a focus on variable selection and Explainable AI (XAI) techniques.  
The study is based on real credit data (Freddie Mac Single-Family Loan-Level Dataset).

### Models
- **`Models.ipynb`**:
  - logistic regression (benchmark),  
  - neural network (MLP),  
  - random forest.  
- **`XGBoost code.ipynb`** – XGBoost implementation with XAI analysis.  
- **`CatBoost code.ipynb`** – CatBoost implementation with XAI analysis.  

### Analysis Scope
- Data preparation and default flag creation (`Data_preparation.ipynb`)  
- Model building and training  
- Evaluation of predictive performance (AUC, ROC, PRC, confusion matrix)  
- Variable selection and comparison across models  
- XAI analyses: SHAP, PDP, error analysis, temporal stability  

---

## Technologies
- Python (pandas, numpy, scikit-learn, matplotlib, seaborn)  
- XGBoost, CatBoost  
- SHAP, PDP  
- DuckDB (data preparation)  

---

## Results
The analyses confirmed the key role of variables such as:  
`credit_score`, `interest_rate`, `dti`, `first_payment_year` – consistently ranked as most important, regardless of the algorithm.
