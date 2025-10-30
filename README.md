# 🚀 IBM Data Science Capstone Project: SpaceX Falcon 9 Launch Success Prediction

![Python](https://img.shields.io/badge/Made%20with-Python-3776AB?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Powered%20by-Jupyter-orange?logo=jupyter)
![Scikit-learn](https://img.shields.io/badge/Scikit--Learn-Modeling-blue?logo=scikitlearn)
![SQLite](https://img.shields.io/badge/SQLite-Database-003B57?logo=sqlite&logoColor=white)
![IBM](https://img.shields.io/badge/IBM%20Certified-Data%20Science%20Professional-006699?logo=ibm)

---

### **Author:** Adam Cunningham  
**Program:** IBM Data Science Professional Certificate  
**Completion Date:** October 2025  

---

## 🧭 Overview

This repository contains my **IBM Data Science Capstone Project**, completed as the final requirement for the **IBM Data Science Professional Certificate**.  

The project simulates a real-world scenario where a fictional competitor, **Space Y**, seeks to estimate SpaceX launch costs by predicting whether Falcon 9 first-stage boosters will successfully land.  
To achieve this, I built an **end-to-end data pipeline** — from **data collection and wrangling** through **exploratory analysis, visualization, and machine learning** — to predict booster recovery outcomes.

---

## 📊 Executive Summary

We achieved an **83.34% prediction accuracy** using classification models built on SpaceX launch data.  
Key findings from the analysis include:

- Booster recovery success can be accurately predicted using features like **Flight Number**, **Orbit**, **Launch Site**, **Payload Mass**, and **Booster Version**.  
- The **K-Nearest Neighbors (KNN)** model demonstrated the best generalization and minimal overfitting.  
- **Interactive dashboards** and **geographic visualizations** revealed additional insights:
  - All launch sites are located **on the coast** and near **transportation infrastructure**.
  - **Kennedy Space Center (KSC)** produced the **most successful recoveries**.
  - Payloads between **3,000–4,000 kg** achieved the **highest success rates**.

---

## 🧩 Project Workflow

### **1. Data Collection**
- Collected launch data using the **[SpaceX REST API](https://github.com/agcunning25-byte/IBM-Data-Science-Capstone-Project/blob/main/jupyter-labs-spacex-data-collection-api.ipynb)**.  
- Supplemented data via **web-scraping Wikipedia** using *BeautifulSoup* ([Notebook Link](https://github.com/agcunning25-byte/IBM-Data-Science-Capstone-Project/blob/main/jupyter-labs-webscraping.ipynb)).

### **2. Data Wrangling**
- Cleaned and transformed data with **SQLite** and **Pandas**.  
- Created a categorical target variable indicating booster landing success.  
- [Data Wrangling Notebook](https://github.com/agcunning25-byte/IBM-Data-Science-Capstone-Project/blob/main/labs-jupyter-spacex-Data%20wrangling.ipynb)

### **3. Exploratory Data Analysis (EDA)**
- Conducted SQL-based insights and statistical exploration ([SQL Notebook](https://github.com/agcunning25-byte/IBM-Data-Science-Capstone-Project/blob/main/jupyter-labs-eda-sql-coursera_sqllite%20(1).ipynb)).  
- Visualized trends and feature relationships using **Seaborn**, **Plotly**, and **Folium**.  
- [EDA Visualization Notebook](https://github.com/agcunning25-byte/IBM-Data-Science-Capstone-Project/blob/main/edadataviz.ipynb)

### **4. Interactive Visualizations**
- Built **Folium maps** to explore launch-site geographies and success/failure clusters.  
  - [Folium Notebook](https://github.com/agcunning25-byte/IBM-Data-Science-Capstone-Project/blob/main/lab_jupyter_launch_site_location%20(1).ipynb)
- Created a **Plotly Dash dashboard** for interactive payload and success analysis.  
  - [Dashboard Notebook](https://github.com/agcunning25-byte/IBM-Data-Science-Capstone-Project/blob/main/spacex_dash_app_py.ipynb)

### **5. Predictive Modeling**
Trained and compared **four supervised classification models** to predict booster landing success:

| Model | Accuracy | Notes |
|--------|-----------|-------|
| Logistic Regression | 83.34 % | Solid baseline model |
| Support Vector Machine | 83.34 % | Balanced and stable |
| Decision Tree | 100 % (train), 66 % (test) | Overfit |
| **K-Nearest Neighbor (KNN)** | **83.34 %** | Best generalization |

- Hyperparameter tuning with **GridSearchCV**  
- Evaluation via **accuracy scores** and **confusion matrices**  
- [Machine Learning Notebook](https://github.com/agcunning25-byte/IBM-Data-Science-Capstone-Project/blob/main/SpaceX_Machine%20Learning%20Prediction_Part_5.ipynb)

---

## 📈 Results

- **Final Model:** KNN Classifier (83.34 % accuracy)  
- **Key Insights:**
  - Orbit types **GEO**, **HEO**, and **SSO** exhibit near-perfect success rates.  
  - Higher payloads tend to correlate with increased success probability.  
  - Coastal launch sites near railways and highways display better recovery outcomes.

---

## 🧠 Conclusions & Next Steps

Although current SpaceX success rates are similar to the model’s predicted accuracy, further optimization could include:

- Applying **stratified sampling** for balanced train/test splits.  
- Introducing **class weights** to handle imbalanced outcomes.  
- Performing deeper hyperparameter tuning on the **Decision Tree** model, which showed strong training accuracy.  

These improvements would enhance recall and reduce false negatives in future iterations.

---

## 🗂️ Repository Structure
**Folder:** IBM-Data-Science-Capstone-Project/
* jupyter-labs-spacex-data-collection-api.ipynb
* jupyter-labs-webscraping.ipynb
* labs-jupyter-spacex-Data wrangling.ipynb
* edadataviz.ipynb
* jupyter-labs-eda-sql-coursera_sqllite (1).ipynb
* lab_jupyter_launch_site_location (1).ipynb
* spacex_dash_app_py.ipynb
* SpaceX_Machine Learning Prediction_Part_5.ipynb
* README.md

---

## 🧰 Tools & Technologies
**Languages:** Python | SQL
**Libraries:** Pandas · NumPy · Seaborn · Plotly · Folium · BeautifulSoup · Scikit-Learn
**Database:** SQLite
**Environment:** Jupyter Notebooks
**API:** SpaceX REST API

---

## 🪙 Key Takeaways
✅ Demonstrates a **complete data science workflow** — from API data collection to ML model deployment.
✅ Combines **SQL analysis, EDA, visualization,** and **machine learning** in one cohesive pipeline.
✅ Integrates **interactive dashboards** and **maps** to communicate findings effectively to stakeholders.

## 📚 Certification Context
This project was developed as the final capstone requirement for the **IBM Data Science Professional Certificate**, showcasing practical expertise across:
* **Data Wrangling & Cleaning**
* **SQL Querying & Exploratory Analysis**
* **Interactive Visualization (Dash & Folium)**
* **Machine Learning Model Building & Evaluation**



## 🏆 Acknowledgments
Special thanks to **IBM**, **Coursera**, and the **SpaceX API maintainers** for providing the tools and data to make this project possible.

© 2025 **Adam Cunningham** — All rights reserved.
