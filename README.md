<h1 align="center"> Chicago SQL Code Summary</h1>
<p align="center">
  
<p align="center">
  <img src="birthsjpg.jpg" width="300" alt="Sublime's custom image"/>
</p>

<p  <img src="https://img.shields.io/badge/Python_Version-3.10%2B-blue" title="Python Version">
  <img src="https://img.shields.io/github/last-commit/dsrichard97/otherprojects">
  <img src="https://img.shields.io/badge/Type_of_ML-NLP-orange">
  <img src="https://img.shields.io/badge/STAT-Algorithms-red">
  <img src="https://img.shields.io/badge/SQL-Descriptive Statistics-brown">
  <img src="https://img.shields.io/badge/STAT-RMSE-blue">
  <img src="https://img.shields.io/badge/Python-Pandas-green">
  <a href="https://github.com/ellerbrock/open-source-badges/"><img src="https://badges.frapsoft.com/os/v1/open-source.svg?v=103"></a>
</p> 


<p>
  <h2>Table of Contents</h2>
  <ul>
    <li><a href="#initial-problem" target="_parent">Identify Issues</a></li>
    <li><a href="#about-the-data">Inspect Data Structure</a></li>
    <li><a href="#data-set-used">Data Selection</a></li>
    <li><a href="#methods">Define Methodology</a></li>
    <li><a href="#tech-stack">Technology Utilization</a></li>
    <li><a href="#quick-glance">Preliminary Findings</a></li>
    <li><a href="#lesson-learned">Insights and Learnings</a></li>
    <li><a href="#limitation">Review Limitations</a></li>
    <li><a href="#notebook">Detailed Analysis</a></li>
    <li><a href="#report">Final Documentation</a></li>
  </ul>
</p>

<P>
  <section id="initial-problem">
    <h2>Identify Issues</h2>
    <p>
Exploring the Impact of Socio-Economic and Racial Factors on Maternal and Infant Health Outcomes in Different Counties


<P>
  <section id="about the data">
    <h2>Inspect Data Structure</h2>
    <p>

This dataset, sourced from the CDC's National Center for Health Statistics, provides detailed statistics on live births in the United States from 2016 to 2022, including demographic and health information derived from birth certificates. It covers a range of data such as mother's race, age, tobacco use, delivery methods, and congenital anomalies. The dataset ensures privacy by suppressing data representing 1-9 births and is a part of the National Vital Statistics System available on the CDC WONDER Online Database. For more information visit: https://wonder.cdc.gov/wonder/help/Natality-expanded.html


## Data Source

An SQL analysis of the relationship between live birth rates in the United States and anomalies from 2016 to 2022, using data from the CDC's National Center for Health Statistics. (Data is gathered from Google BigQuery)

 [Data Analysis Question & Answers](questions_and_answers.md)

<P>
  <section id="data set used">
    <h2>Data Set Used</h2>
    <p>
Seven key [datasets](datasets.md) for this case study

![alt text](picdataset.png)

## Entity Relationship Diagram

![alt text](in1.png)

<P>
  <section id="methods">
    <h2>Methods</h2>
 
- Exploratory Data Analysis
- Multivariate Analysis
- Visualizations
- Modeling
- Reporting




<P>
  <section id="tech-stack">
    <h2>Tech Stack</h2>
    
  - **SQL** (Scrapping Data)
  - **R** (Further investigation)
  - **Tableau**  (Visuals)
  - **Github** (Reporting & Reproduce)


<P>
  <section id="quick-glance">
    <h2>Quick glance at the Results</h2>
 <p>
   Distribution
   
<p align="center">
  <img src="distrib.png" width="300" alt="Sublime's custom image"/>
</p>

Correlation Matrix
<p align="center">
  <img src="corr.png" width="300" alt="Sublime's custom image"/>
</p>
Initial Correlation Assessment:
The heatmap of the correlation matrix provides insights into how these variables are related to each other. For instance, a positive correlation between maternal age and birth weight could suggest that older mothers tend to have babies with higher birth weights.

Predictive Modeling:
Used Random Forest model to identify significant predictors.
Found average birth weight, maternal age, pre-pregnancy BMI, and prenatal weeks as critical factors.
- Average Birth Weight (grams): 2429.82. This was the most significant predictor.
- Average Age of Mother: 2290.50. This was a strong predictor, second only to birth weight.
- Average Pre-pregnancy BMI: 2243.89. Another important predictor​​.

ML Algorithm Accuracy:
Compared radial, sigmoid, and polynomial kernel functions in SVM.
Radial kernel function performed best in terms of RMSE, indicating its effectiveness in modeling high-risk pregnancies.

Root Mean Square Error (RMSE):
- Radial Kernel Function -> 8296.19
- Polynomial Kernel Function -> 12857.87
- Sigmoid Kernel Function -> 16844.82​​

<P>
  <section id="limitation">
    <h2>Limitation and what can be Improved</h2
                                             
- Data Scope: Limited to U.S. data; expanding the data set to include global statistics could offer more comprehensive insights.
- Model Diversity: Explore additional machine learning models beyond Random Forest and SVM for potentially better predictions or insights.
- Feature Engineering: Experiment with more complex features or interactions between variables to enhance model performance.
- Real-Time Data Integration: Incorporate real-time data updates for more dynamic and current analyses.
- User Interface: Develop an interactive dashboard for easier access and interpretation of results by non-technical users.


This project offers valuable insights into maternal and infant health, leveraging advanced data analytics and machine learning techniques. Future work could expand the dataset, explore new models, and enhance user interaction to increase the impact and reach of the findings.
   
<P>
  <section id="notebook">
    <h2>Explore the notebook</h2
 <p>
To explore the R notebook file click here: (https://github.com/dsrichard97/cdc_births/blob/main/cdcsummary.pdf).

<P>
  <section id="report">
    <h2>Report and Presentation</h2
 <p>

