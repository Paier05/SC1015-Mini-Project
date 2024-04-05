# SC1015-Mini-Project_FDDC_Group1
# Overview
With the development of modern society and the change in lifestyle, diabetes, as one of the most prevalent chronic diseases, shows signs of rejuvenation. According to an article by CNA(2023), the number of diabetes patients who are 30 years old is increasing at an alarming rate nowadays. Based on the report by Diabetes Singapore (2022), the number of people with diabetes is estimated to grow up to 1 million by the year 2050. This accounts for 10% of disease burdens in Singapore. Hence, diabetes prevention and early detection to prevent and diagnose diabetes is crucial. <br><br>
Our project aims to predict the probability of one getting diabetes by different variables. By this, we hope to provide insights for people to adopt a healthier lifestyle and raise awareness among the public on diabetes prevention and early detection.
# Dataset
The dataset used can be found <a href = "https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset?select=diabetes_012_health_indicators_BRFSS2015.csv" >here</a>. <br>
The dataset provides approximately 245k survey responses on diabetes collected by the Centers for Disease Control and Prevention (CDC) under the Behavioral Risk Factor Surveillance System (BRFSS). A detailed explanation of the feature variables in the dataset can be found <a href = "https://github.com/Paier05/SC1015-Mini-Project/blob/main/0.%20Description%20of%20Variables.xlsx">here</a>.
# Methodology
<h3 href = "https://github.com/Paier05/SC1015-Mini-Project/blob/main/Data%20Cleaning.ipynb">1. Data Cleaning</h3>
We modified the data types of different variables so that it was easier for us to carry out the data analysis. We also found that there is a significant unbalance between the amount of data for diabetes and non-diabetes patients. In order to make the amount of data equal for more efficient analysis, we used the `undersampling` method to reduce the amount of data for non-diabetes patients. Lastly, we export the new dataset as `resampled.csv`.
<h3 href = "https://github.com/Paier05/SC1015-Mini-Project/blob/main/EDA.ipynb">2. Exploratory Data Analysis</h3>
After cleaning up and modifying the data, we proceed to find suitable variables for our model training. We first explore the relation of variables (both numerical and categorical) with the status of diabetes by visualizing it in graphs. After analyzing the graphs plotted, we sorted out the suitable variables for our use. Then, observing that the outliers of BMI may affect our model training, we removed the outliers before exporting it as a new dataset `diabetes_EDA.csv`.
<h3 href = "https://github.com/Paier05/SC1015-Mini-Project/blob/main/Machine%20Learning.ipynb">3. Machine Learning</h3>
We analyze our data by using different models:<br>
- Logistic Regression<br>
- Random Forest<br>
- Gradient Boosting<br>
We also evaluate on the importance of features affecting the prediction of diabetes in each model and compare the accuracy of the models.

# Results
After comparing the three models we used, we found that the accuracy of the three models are almost the same. However, as shown in the graph, the training accuracy of the random forest model is significantly the highest. From our discussion, this might be due to overfitting of the training dataset. Learning from the feature importance graph, we get the following order of importance for each model:
||Log | Random | Gradient | 
| --- | --- | --- |--- |
|Top 1 | HighBP | BMI | HighBP | 
|Top 2 | HighChol | Age | GenHlth |
|Top 3 | GenHlth | Income | BMI | 
|Top 4 | HeartDiseaseorAttack | GenHlth | Age | 
|Top 5 | Age | PhysHlth | HighChol |

Thus, we conclude that the top 8 important factors to predict diabetes are:

- HighBP
- BMI
- HighChol
- Age
- GenHlth
- Income
- HeartDiseaseorAttack
- PhysHlth

# Conclusion
Nowadays, people are more and more concerned about diabetes as it is detrimental to our daily lives if we have it. Comparing all the factors causing diabetes, we could find that most of the factors that are highly relevant to diabetes actually can be controlled by ourselves. Even changing the different models, the factors causing diabetes are almost the same. As such, diabetes, or other chronic diseases, should be should be prevented by ourselves but not controlled by medicine after having those diseases.

# What did we learn from this project? 
- Impact of unbalanced dataset
- The use of undersampling and oversampling to due with imbalanced data
- New models for machine learning (logistic regression, random forest, gradient boosting)
- Project contribution through GitHub
- The impact of overfitting
- The main factors causing diabetes, and the awareness of taking care of our health

# Contributors
Tan Ming Hao (@Paier05) - Data Visualisation, Exploratory Data Analysis, Overall Presentation <br>
Cho Zhi Wei (@ChoWei0310) - Data Cleaning, Exploratory Data Analysis, Overall Presentation <br>
Lai Xin Yee (@CLXYee) - Exploratory Data Analysis, Machine Learning, Feature Extraction <br>

# References
- https://www.diabetesatlas.org/data/en/country/179/sg.html
- https://www.diabetes.org.sg/about-diabetes/the-singapore-demographics-of-diabetes/
- https://semaphoreci.com/blog/imbalanced-data-machine-learning-python
- https://www.channelnewsasia.com/singapore/war-against-diabetes-singapore-doctors-seeing-rise-young-patients-below-40-lifestyle-habits-stress-early-screening-treatment-3921976 
