# Nata Visionaries – Machine Learning Quality Classification
Final Project | Machine Learning I | NOVA IMS

This project was developed as the **Group Project for the Machine Learning I course** in the **Bachelor in Data Science at NOVA IMS (2025–2026)**.

The objective is to build a **machine learning model capable of predicting the quality of a Pastel de Nata** based on production and recipe characteristics.

---

# Project Objective

The **Nata Visionaries Brotherhood** collected production data from bakeries in **Porto and Lisbon** to determine what makes a perfect **Pastel de Nata**.

Currently, the evaluation process used to determine pastry quality is **destructive**, meaning the pastry must be destroyed during the evaluation.

The objective of this project is therefore to develop a **classification model** that predicts whether a pastry is:

- **OK** – High quality, approved by the Nata Visionaries  
- **KO** – Acceptable but below the desired standard  

By predicting quality using production data, bakeries can:

- Reduce waste caused by destructive testing  
- Improve recipes and baking processes  
- Maintain consistent product quality  

The evaluation metric used for the model is **Accuracy**.

---

# Dataset Description

The dataset contains **production measurements and recipe parameters** for each Pastel de Nata.

## Features

| Feature | Description |
|------|------|
| origin | Bakery location (Porto or Lisbon) |
| preheating time | Oven preheating duration |
| baking duration | Baking time at high temperature |
| cooling period | Resting time after baking |
| sugar content | Sugar in custard filling |
| salt ratio | Salt concentration in pastry |
| egg temperature | Temperature of eggs when added |
| oven temperature | Final baking temperature |
| cream fat content | Fat percentage of cream |
| lemon zest ph | pH level of lemon zest infusion |
| vanilla extract | Concentration of vanilla extract |
| egg yolk count | Number of egg yolks used |

## Target Variable

| Variable | Description |
|------|------|
| quality class | Final pastry quality classification (**OK / KO**) |

---

# Project Methodology

The project follows an adapted **CRISP-DM methodology**.

## 1. Data Understanding
- Explore dataset structure and feature distributions  
- Identify missing values and inconsistencies  
- Detect potential outliers  

## 2. Data Preprocessing
- Handle missing values  
- Encode categorical variables (e.g., origin)  
- Scale numerical variables  
- Prepare the dataset for modeling  

## 3. Feature Engineering
- Analyze feature importance  
- Create new relevant features  
- Remove redundant or low-impact variables  

## 4. Modeling

Several classification algorithms are tested, such as:

- Logistic Regression  
- Decision Trees  
- Random Forest  
- K-Nearest Neighbors  
- Support Vector Machines  

Models are evaluated using **Accuracy**.

## 5. Hyperparameter Tuning

Optimization techniques are used to improve model performance:

- Grid Search  
- Cross-Validation  

## 6. Final Model & Prediction

The best performing model is used to:

- Generate predictions for the **predict.csv** dataset  
- Submit predictions to the **Kaggle competition**

---

# Project Structure

pasteis_de_nata
│
├── Data
│   ├── data_dictionary.csv
│   ├── learn.csv
│   ├── predict.csv
│   └── sampred.csv
│
├── Final Project
│   ├── Data
│   ├── ML07_NB1_DATAEXPLORATION.ipynb
│   ├── ML07_NB2_PREP_FEAT_MODEL.ipynb
│   └── ML07_NB9_FINAL.ipynb
│
├── Project Description.pdf
│
└── README.md

---

# Technologies Used

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  

---

# Model Output

The final model generates predictions in the format required for the **Kaggle competition submission**, classifying each pastry as:

- **OK**
- **KO**

---

# Authors

Carolina Arez  
Henrique Madureira  
Miguel Melo  
Noa Penas  

Bachelor in Data Science  
NOVA IMS – Information Management School
