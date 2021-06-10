# Disease-Prediction
<h3>Team Members</h3><br/>  
(a) Kaustav Deb<br/>  
(b) Sayantika Chakravarty<br/>  
(c) Oiendrila Basak <br/>
<h3>Domain:</h3><br/>
Pharma<br/>
<h3>AIM:</h3><br/>
To predict the occurence of a stroke based on a number of personal details provided<br/>
Data: obtained from Kaggle on stroke<br/>
Data link: https://www.kaggle.com/fedesoriano/stroke-prediction-dataset<br/>
<h3> Problem statement </h3><br/>
To predict whether a patient is likely to get stroke based on the input parameters like gender, age, various diseases, and smoking status. Each row in the data provides relavant information about the patient.
<h3>Data Description</h3><br/>
The dataset has 5111 rows and 12 columns.
<h3>Software:</h3>Python
<h3>Attribute Information</h3><br/>
1) id: unique identifier of an individual<br/>
2) gender: "Male", "Female" or "Other"<br/>
3) age: age of the patient<br/>
4) hypertension: 0 if the patient doesn't have hypertension, 1 if the patient has hypertension<br/>
5) heart_disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease<br/>
6) ever_married: Marital status of the individual. "No" or "Yes"<br/>
7) work_type: "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"<br/>
8) Residence_type: "Rural" or "Urban"<br/>
9) avg_glucose_level: average glucose level in blood<br/>
10) bmi: body mass index<br/>
11) smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"*<br/>
12) stroke: 1 if the patient had a stroke or 0 if not<br/>
*Note: "Unknown" in smoking_status means that the information is unavailable for this patient<br/>
<h3>Statistical Methods</h3><br/>
<h4>Data Handling</h4><br/>
After importing the data set in python we first drop the id column as it plays no role in predicting whether a person will suffer from stroke or not.After that we check for null values in the data set and find that the bmi column has 201 null values, we replace those null values by the mean value. Then we find out the data summary to have a rough idea of the population we are dealing with, the average age group, the average bmi etc.
<h4>Exploratory Data Analysis</h4><br/>
 We visualize the different categorical features (hypertension, heart_disease,gender,smoking status,marital status,area of residence,occupation) using countplot and we draw boxplots for the continuous variables(age,bmi,average glucose level). These graphical representations will give us an idea of the effect these factors have on the target variable. <br/>
 We also plot a histogram to obtain the frequency distribution of the continuous variables.<br/>
 We use the corr() function to get the measure of correlation between different numerical factors and we plot this rectangular data as a color-encoded matrix using heatmap where the darker shades of colour represent a lower value than lighter shades.<br/>
 We use pairplot to plot pairwise relationships in a dataset. By default, this function will create a grid of Axes such that each numeric variable in data will by shared across the y-axes across a single row and the x-axes across a single column. The diagonal plots are treated differently: a univariate distribution plot is drawn to show the marginal distribution of the data in each column.<br/>
 <h3>Discussion</h3><br/>
To do the EDA properly.
<h3>Questions</h3><br/>
1. how do we decide which outliers to drop and which to keep.<br/>
2. 
