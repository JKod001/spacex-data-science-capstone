# spacex-data-science-capstone

## Project Overview
This project is the final capstone for the IBM Data Science Professional Certificate.  
The objective is to analyze historical SpaceX launch data and build predictive models to determine whether a Falcon 9 first-stage booster will successfully land.

Successful booster recovery is a key factor in reducing launch costs, making landing prediction an important operational and business problem.

---

## Objectives
- Collect SpaceX launch data using APIs and web scraping
- Perform exploratory data analysis (EDA) using visualization and SQL
- Build interactive maps and dashboards
- Train and evaluate machine learning models to predict landing success
- Compare model performance and select the best approach

---

## Data Sources
- SpaceX REST API (launch, payload, booster data)
- Wikipedia (historical launch records)
- IBM Skills Network datasets

---

## Methodology

### Data Collection & Wrangling
- Merged data from multiple sources
- Handled missing values and inconsistent categories
- Encoded categorical features
- Created a binary target variable (`Class`)

### Exploratory Data Analysis
- Visual analysis of payload mass, orbit type, and launch site
- SQL-based aggregation and filtering
- Temporal trends in launch success rates

### Visualization
- Interactive maps using Folium
- Interactive dashboard using Plotly Dash
- Payload vs success scatter plots
- Launch site success breakdowns

### Machine Learning
The following classification models were trained and evaluated:
- Logistic Regression
- Support Vector Machine (SVM)
- Decision Tree
- K-Nearest Neighbors (KNN)

Hyperparameters were tuned using `GridSearchCV`, and models were evaluated using a held-out test set.

---

## Results
- All models achieved similar test accuracy (~83%)
- Confusion matrices showed strong performance for successful landings
- Logistic Regression was selected as the final model due to:
  - Comparable accuracy
  - Interpretability
  - Simplicity and stability

---

## Conclusion
Payload mass, orbit type, and launch site are strong predictors of landing success.  
The results demonstrate that simpler models can perform as well as more complex ones when the dataset is small and well-structured.

Future improvements could include:
- Weather data integration
- Real-time telemetry
- Larger historical datasets

---

## Files in This Repository
- Jupyter notebooks for each project stage
- Plotly Dash application (`spacex-dash-app.py`)
- Final presentation (PowerPoint & PDF)
- Processed datasets

---

## Tools & Libraries
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Folium
- Plotly Dash

---

## Author
Justin Kodurand  
IBM Data Science Capstone Project
