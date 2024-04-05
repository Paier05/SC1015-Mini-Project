# SC1015-Mini-Project_FDDC_Group1
# Contributors
Tan Ming Hao (@Paier05) - <br>
Cho Zhi Wei (@ChoWei0310) - <br>
Lai Xin Yee (@CLXYee) - <br>
# Overview
With the development of modern society and the change in lifestyle, diabetes, as one of the most prevalent chronic diseases, shows signs of rejuvenation. Based on the report by Diabetes Singapore (2022), the number of people with diabetes is estimated to grow up to 1 million by the year 2050. This accounts for 10% of disease burdens in Singapore. Hence, diabetes prevention and early detection to prevent and diagnose diabetes is crucial. <br><br>
Our project aims to predict the probability of one getting diabetes by different variables. By this, we hope to provide insights for people to adopt a healthier lifestyle and raise awareness among the public on diabetes prevention and early detection.
# Dataset
The dataset used can be found <a href = "https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset?select=diabetes_012_health_indicators_BRFSS2015.csv" >here</a>. <br>
The dataset provides approximately 245k survey responses on diabetes collected by the Centers for Disease Control and Prevention (CDC) under the Behavioral Risk Factor Surveillance System (BRFSS). Detailed explanation of the feature variables in the dataset can be found <a href = "https://github.com/Paier05/SC1015-Mini-Project/blob/main/0.%20Description%20of%20Variables.xlsx">here</a>.
# Methodology
<h3 href = "https://github.com/Paier05/SC1015-Mini-Project/blob/main/Data%20Cleaning.ipynb">1. Data Cleaning</h3>
We modified the data types of different variables so that it is easier for us to carry out the data analysis. We also found that there is a significant unbalance between the amount of datas for diabetes and non-diabetes patients. In order to make the amount of data equal for more efficient analysis, we used the `undersampling` method to reduce the amount of datas for non-diabetes patients. Lastly, we export the new dataset as `resampled.csv`.
<h3 href = "https://github.com/Paier05/SC1015-Mini-Project/blob/main/EDA.ipynb">2. Exploratory Data Analysis</h3>
After cleaning up and modifying the data, we proceed to find suitable variables for our model training. We first explore the relation of variables (both numerical and categorical) with the status of diabetes by visualizing it in graphs. After analysing the graphs plotted, we sorted out the suitable variables for our use. Then, observing that the outliers of BMI may affect our model training, we removed the outliers before exporting it as a new dataset `diabetes_EDA.csv`.
<h3 href = "https://github.com/Paier05/SC1015-Mini-Project/blob/main/Machine%20Learning.ipynb">3. Machine Learning</h3>
We analyse our data by using different models:<br>
- Logistic Regression<br>
- Random Forest<br>
- Gradient Boosting<be>

# Results
# Conclusion
# What we learn from this project? 
- The use of undersampling and oversampling to due with imbalance datas
- New models for machine learning (logistic regression, random forest, ...)
- Project contribution through GitHub
- The impact of overfitting
- The main factors causing diabetes, and the awareness of taking care of our health
# References
- https://www.diabetesatlas.org/data/en/country/179/sg.html
- https://www.diabetes.org.sg/about-diabetes/the-singapore-demographics-of-diabetes/
- https://semaphoreci.com/blog/imbalanced-data-machine-learning-python
