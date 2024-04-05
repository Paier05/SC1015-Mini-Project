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
The dataset provides approximately 245k survey responses on diabetes collected by the Centers for Disease Control and Prevention (CDC) under the Behavioral Risk Factor Surveillance System (BRFSS). Detailed explanation of the feature variables in the dataset can be found <a href = "https://github.com/Paier05/SC1015-Mini-Project/blob/main/Description%20of%20Variables.xlsx">here</a>.
# Methodology
<h3 href = "https://github.com/Paier05/SC1015-Mini-Project/blob/main/Data%20Cleaning.ipynb", style = "color:red">1. Data Cleaning</h3>
Since our original dataset is huge, we reduced the size of our dataset by half through random split. We also did some modifications to the data for us to work on the machine learning more efficiently.
<h3 href = "https://github.com/Paier05/SC1015-Mini-Project/blob/main/EDA.ipynb", style = "color:red">2. Exploratory Data Analysis</h3>
After doing some modifications to our data, on this topic, we aim to find suitable data for our model training. We first explore the correlation of variables (both numerical and categorical) with the status of diabetes by visualizing it in the graph. After learning every graph plotted, we sorted out the suitable variables for our use which are `"HighBP", "HighChol", "Sex", "PhysActivity", "DiffWalk", "BMI", "GenHlth", "PhysHlth", "Age", "Income"`. Then, observing that the outliers of BMI may affect our model training, we clean the outliers. 

# Results
# Conclusion
# What we learn from this project? 
# References
- https://www.diabetesatlas.org/data/en/country/179/sg.html
- https://www.diabetes.org.sg/about-diabetes/the-singapore-demographics-of-diabetes/
