# IBM-Data-Science-Capstone-Project
A capstone project from the IBM Data Science professional certificate on Coursera
SpaceX Falcon 9 Landing Prediction Project

![Python](https://img.shields.io/badge/Python-3.9-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-ScikitLearn-orange)
![Dashboard](https://img.shields.io/badge/Dashboard-Plotly%20Dash-purple)
![Visualization](https://img.shields.io/badge/Visualization-Seaborn-green)
![Project](https://img.shields.io/badge/Coursera-IBM%20Data%20Science-blue)




# SpaceX Falcon 9 Landing Prediction Project

![Python](https://img.shields.io/badge/Python-3.9-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-ScikitLearn-orange)
![Dashboard](https://img.shields.io/badge/Dashboard-Plotly%20Dash-purple)
![Visualization](https://img.shields.io/badge/Visualization-Seaborn-green)
![Project](https://img.shields.io/badge/Coursera-IBM%20Data%20Science-blue)

---

# **Project Overview**

This project analyzes historical **SpaceX Falcon 9 launch data** to identify patterns that influence the success of first-stage landings and to build predictive models capable of forecasting landing outcomes.

SpaceX significantly reduces launch costs by reusing the Falcon 9 first stage. Predicting whether the first stage will land successfully helps estimate launch costs and mission feasibility.

In this project, publicly available data was collected, processed, analyzed, and used to train machine learning models that predict the probability of successful rocket landings.

---

# **Objectives**

The main objectives of this project were to:

• Collect launch data using the **SpaceX REST API**
• Extract historical launch data using **web scraping**
• Perform **data wrangling and preprocessing**
• Conduct **exploratory data analysis (EDA)**
• Query launch data using **SQL**
• Build **interactive geospatial visualizations**
• Create an **interactive dashboard**
• Develop and evaluate **machine learning classification models**

---

# **Data Sources**

The dataset used in this project was collected from two primary sources.

## **1. SpaceX REST API**

The SpaceX API provided structured launch data including:

• Flight number
• Launch site
• Payload mass
• Orbit type
• Booster version
• Landing outcome

The API responses were converted from JSON format into structured datasets using **pandas.json_normalize()**.

---

## **2. Web Scraping**

Additional launch data was scraped from the **Falcon 9 Wikipedia launch records page** using:

• Requests
• BeautifulSoup

The extracted tables were cleaned and merged with the API dataset.

---

# **Data Wrangling**

The collected datasets required preprocessing before analysis.

Key data wrangling steps included:

• Handling missing values
• Removing duplicates
• Converting categorical variables into numerical features
• Creating a binary target variable indicating landing success
• Feature scaling for machine learning models

The cleaned dataset was then used for analysis and predictive modeling.

---

# **Exploratory Data Analysis (EDA)**

Exploratory data analysis was performed using both **data visualization** and **SQL queries**.

## **Visualization Insights**

Several visualizations were created to explore the dataset, including:

• Flight Number vs Launch Site
• Payload Mass vs Launch Site
• Success Rate by Orbit Type
• Flight Number vs Orbit Type
• Payload vs Orbit Type
• Yearly Launch Success Trend

The analysis revealed that **launch success rates improved significantly over time**, reflecting improvements in SpaceX landing technology.

---

## **SQL Analysis**

SQL queries were used to answer key questions such as:

• Identifying all unique launch sites
• Finding launches from CCAFS launch sites
• Calculating total payload mass carried by NASA missions
• Determining the first successful landing on a ground pad
• Ranking landing outcomes across time periods

---

# **Interactive Visual Analytics**

## **Folium Map**

An interactive map was created using **Folium** to visualize launch site locations.

The map included:

• Launch site markers
• Color-coded launch outcomes
• Distance calculations to nearby infrastructure such as railways, highways, and coastlines

This geospatial analysis helped understand geographic factors affecting launch operations.

---






---

# **Predictive Analysis**

Machine learning models were developed to predict whether the Falcon 9 first stage would successfully land.

The following classification models were evaluated:

• Logistic Regression
• Support Vector Machine (SVM)
• Decision Tree
• K-Nearest Neighbors (KNN)

Model tuning was performed using **GridSearchCV** to identify the best hyperparameters.

---

# **Model Performance**

| Model                  | Accuracy |
| ---------------------- | -------- |
| Logistic Regression    | 83.33%   |
| Support Vector Machine | 83.33%   |
| K-Nearest Neighbors    | 83.33%   |
| Decision Tree          | ~86%     |

The **Decision Tree model achieved the highest accuracy**, making it the best performing model for predicting landing outcomes.

---

# **Project Architecture**

The project follows a complete **end-to-end data science pipeline**.

```
Data Collection
      ↓
SpaceX REST API + Web Scraping
      ↓
Data Wrangling
      ↓
Exploratory Data Analysis
(Visualization + SQL)
      ↓
Interactive Visual Analytics
(Folium Maps + Plotly Dash Dashboard)
      ↓
Machine Learning Model Development
(Logistic Regression, SVM, Decision Tree, KNN)
      ↓
Model Evaluation
      ↓
Landing Outcome Prediction
```

---

# **Technologies Used**

Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
BeautifulSoup
Folium
Plotly Dash
SQL

---

# **Repository Structure**

```
SpaceX-Falcon9-Prediction
│
├── notebooks
│   ├── spacex-data-collection-api.ipynb
│   ├── webscraping.ipynb
│   ├── data-wrangling.ipynb
│   ├── eda-visualization.ipynb
│   ├── eda-sql.ipynb
│   ├── folium-map.ipynb
│   ├── machine-learning-prediction.ipynb
│
├── dashboard
│   └── spacex-dash-app.py
│
├── data
│
├── presentation
│   └── SpaceX_Capstone_Presentation.pdf
│
└── README.md
```

---

# **Key Findings**

• Launch success rates improved significantly over time.
• Payload mass and orbit type influence landing outcomes.
• Launch site characteristics affect mission success.
• Machine learning models can effectively predict Falcon 9 landing success.

---

# **Conclusion**

This project demonstrates how data science techniques can be applied to aerospace datasets to uncover insights and build predictive models.

By analyzing historical SpaceX launch data, we identified patterns influencing landing success and developed machine learning models capable of predicting Falcon 9 first-stage landing outcomes with high accuracy.

---

✅ This version will look **clean and professional on GitHub**.

---

If you want, I can also show you **one extremely important section that most students forget in their README but graders love** (it will make your repository look **much more like a professional data science project**).

Conclusion

This project demonstrates how data science techniques can be applied to aerospace datasets to uncover insights and build predictive models. By analyzing historical SpaceX launch data, we identified patterns influencing landing success and developed a machine learning model capable of predicting Falcon 9 first-stage landing outcomes with high accuracy.
