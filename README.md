# 🫀 Heart Disease Risk Prediction using Bayesian Networks

A data-driven probabilistic model built to predict heart disease risk using a simulated patient dataset and Bayesian Networks via the `pgmpy` library. This project demonstrates data cleaning, probabilistic graphical modeling, and inference techniques in a healthcare scenario.

---

## 📌 Problem Statement

As a Data Detective at **MediMystery Labs**, your mission was to predict the risk of heart disease based on patient medical records.  
Using Bayesian Networks, the model computes the probability of heart disease and other health parameters under certain conditions.

---

## 📊 Approach

1. **Data Cleaning**
   - Loaded patient data from `heart_disease.csv`.
   - Removed duplicate records.
   - Handled missing values by dropping incomplete rows.
   - Applied **Min-Max Normalization** to continuous columns for consistent scaling.

2. **Bayesian Network Construction**
   - Defined a Bayesian Network structure with relationships:
     ```
     age → fbs → target → (chol, thalach)
     ```
   - Built and trained the model using **Maximum Likelihood Estimation (MLE)**.

3. **Probabilistic Inference**
   - Queried the model to:
     - Compute the probability of heart disease.
     - Visualize the probability distribution of cholesterol levels.
     - Perform conditional inference based on patient parameters.

4. **Visualization**
   - Visualized the Bayesian Network structure using `networkx`.
   - Displayed inference results as bar plots using `seaborn` and `matplotlib`.

---

## 📦 Libraries Used  

| Library          | Purpose                          |
|:----------------|:---------------------------------|
| `pandas`         | Data manipulation and preprocessing |
| `numpy`          | Numerical operations             |
| `sklearn`        | Min-Max Normalization             |
| `pgmpy` `1.0.0`  | Bayesian Network modeling and inference |
| `networkx`       | Graph creation and visualization  |
| `matplotlib`     | Data visualization                |
| `seaborn`        | Enhanced plotting for inference results |

---

## 🔧 Installation  

Install the required libraries using:

```bash
pip install pandas numpy scikit-learn pgmpy==1.0.0 networkx matplotlib seaborn
````

---

## 📈 Outputs

* ✅ Cleaned and normalized patient dataset
* ✅ Trained Bayesian Network model
* ✅ Probability of heart disease occurrence
* ✅ Cholesterol distribution plot
* ✅ Bayesian Network structure diagram

---

## 📂 Dataset

* `heart_disease.csv` — simulated patient health records with attributes like age, cholesterol, fasting blood sugar, thalach (max heart rate), etc.

---

## 📌 Future Improvements

* Discretize continuous variables into categorical bins for better model stability.
* Extend to more complex probabilistic inference queries.
* Integrate with a Streamlit dashboard for interactive exploration.

---

## 📜 License

Open for educational and demonstration purposes.

---

## 🙌 Acknowledgements

This project was part of a Data Science challenge at **COSC Hackweek**.

```

---
