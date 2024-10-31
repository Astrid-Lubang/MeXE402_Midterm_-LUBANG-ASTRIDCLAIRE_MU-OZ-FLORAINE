# TABLE OF CONTENTS
  * [I. INTRODUCTION](#i-introduction)
  * [II. DATASET DESCRIPTION](#ii-datasetdescription)
  * [III. PROJECT OBJECTIVES](#iii-projectobjectives)
  * [IV. DOCUMENTATION](#iv-documentation) <br>
      + [ METHODOLOGY](methodology) <br>
  * [V.SUMMARY AND FINDINGS](v.summaryandfindings)
  * [VI.REFERENCE](#vi-reference)
    
# I. INTRODUCTION

+ ***SALES DATA*** <br>
 <p align="justify"> 
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This dataset appears to capture sales transactions, including information about orders, customers, and sales revenue. Each row represents a specific order line item, with details such as the order number, quantity ordered, price per item, and the total sales value for that line. In addition to transactional data, the dataset includes metadata like order date, order status, and various categorical fields such as the type of product, the deal size, and customer information. Some key columns include SALES, which reflects the total sales revenue from each transaction, and QUANTITY ORDERED and PRICE EACH, which provide insights into product pricing and order volume.The goal is to provide data insights to support business decision making and improve sales strategies. 
 <br>

 <p align="justify"> 

 + ***BREAST CANCER WISCONSIN*** <br>

  <p align="justify"> 
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The "Breast Cancer Wisconsin" notebook provides a detailed look at using logistic regression to detect breast cancer. It starts with thorough data preparation, including importing key libraries (Pandas, Scikit-Learn) for handling and modeling data. The dataset, called LOGISTIC.csv, is cleaned by removing unnecessary columns and addressing missing values to keep the data accurate. The target variable diagnosis is also converted to numbers for easier processing. After cleaning, the notebook divides the data into input features and target labels to set up for logistic regression modeling, following best practices. This step-by-step approach guides readers through each part, highlighting accurate breast cancer prediction and demonstrating how predictive modeling can support healthcare diagnostics. <br>
 

# II.DATASET DESCRIPTION
<p align="justify"> 
 
 + ***SALES DATA*** <br>
 <p align="justify"> 
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  This table shows the  outlines of the variable and its characteristics contained in the sales dataset. Each variables serve a significant function in analyzing the sales performance.
 
<div align="center">

 |  **VARIABLE** |  **DESCRIPTIONS** |
 |:-|:-|
 |   **Order Number**   |   Unique identifier for each order.  |
 |   **Quantity Ordered**   |   Number of units ordered. |
 |   **Price Each**   | Price per unit. |
 |   **Sales**   | Total sales amount (dependent variable for potential analysis).j |
 |   **Order Date**   | Date when the order was placed.. |
 |   **Order Number**   | Number of units ordered. |
 |   **STATUS**   | Shipping status of the order.4ree |
 |   **QTR_ID, MONTH_ID, YEAR_ID**   | Identifiers for the quarter, month, and year of the order. |
 |   **Country**   | Country where the order was shipped. |
 |   **Deal Size**   | Size of the deal (Small, Medium, Large). |
 
<p align="center"> 
 
***Table 1:Variables used in dataset in Sales Data***
</div>
<br>

<p align="justify"> 

 + ***BREAST CANCER WISCONSIN*** <br>
 <p align="justify"> 
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  This table shows the  outlines of the variable and its characteristics contained in the breast cancer wisconsin dataset. Each variable serves a significant function in analyzing the tumor characteristics and aiding in the diagnosis classification.<br>
  
 <div align="center">

 |  **VARIABLE** |  **DESCRIPTIONS** |
 |:-|:-|
 |   **ID**   |   Unique identifier for each observation.  |
 |   **Diagnosed**   |   Diagnosis outcome ('M' for malignant, 'B' for benign). |
 |   **Raduis_Mean**   | Mean radius of cells. |
 |   **Texture_Mean**   | Mean texture (variance in grayscale values). |
 |   **Perimeter_Mean**   | Mean perimeter of cells. |
 |   **Area_Mean**   | Mean area of cells. |
 |   **Smoothness_mean**   | Mean smoothness (local variation in radius) |
 |   **Compactness_Mean**   | Mean compactness (perimeter² / area - 1.0). |
 |   **Concavity_Mean**   | Mean concavity (severity of concave portions). |
 |   **Concave points_Mean**   |   Mean number of concave points on cells.. |
 |   **Fractal_Dimension_Mean**   |  Mean fractal dimension (coastline approximation). |
 
<p align="center"> 
 
***Table 2:Variables used in Breast Cancer Wisconsin dataset***
</div>
<br>
 

# III. PROJECT OBJECTIVES
<p align="justify"> 

 + ***Sales Data*** <br>
Following are the project objectives:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1. Clean and prepare the dataset.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2. Investigate key sales metrics and patterns to understand underlying trends.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3. Identify and select influential features that may affect sales performance.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4.: Apply linear regression to predict sales outcomes based on various features.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 5.Assess the model’s accuracy and reliability in predicting sales by examining performance metrics.<br>

<p align="justify"> 
 
 + ***BREAST CANCER WISCONSIN*** <br>
Following are the objectives for Breast Cancer Wisconsin dataset:<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1.To clean, prepare and structure the dataset effectively for analysis<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2.To examine and select the relevant features that impact tumor classification.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3.To apply logistic regression for classifying tumors as malignant or benign.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4. To assess the model’s performance using accuracy, precision, and other relevant metrics.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 5. To provide diagnostic insights into breast cancer cases by analyzing feature contributions and model outcomes.<br>
 
# IV. DOCUMENTATION
 <h1 align="justify">METHODOLOGY</h1>
     
 <h1 align="center">LINEAR REGRESSION: SALES DATA</h1>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; The following steps outline the methodology used for the analysis of the "Sales Data". Each step is designed to understand the dataset:
<br>

<h1 align="justify">Part 1: Data Processing</h1>
 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **1.1 Importing Datasets** 
 <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/a42ea2b9-eca7-458d-a94a-a582dd4aad67"style=  "height: 180px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  **1.2 HANDLE MISSING VALUES**
  <br>
 <p align="justify"> 
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; In this part the process involves indentifying and addressing any gaps in dataset. This may include the checking missing values and dropping the missing values.The figures attached are the step by step process. <br>
  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  **Checking Missing Values** <br>  
+ The "ADDRESSLINE2," "STATE," "POSTALCODE," and "TERITORY" categories have multiple missing variables. <br>
  
<p align="center">
<img src= "https://github.com/user-attachments/assets/756a67c0-a05d-446a-9c5e-235641e64c13"style=  "height: 300px;"> <br>

  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  **Dropping Missing Values** <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/15521807-1cd3-4bb6-8a2b-7197c37cc3a9" style= "height: 300px;"> 
  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **1.3 CHECK FOR OUTLIERS**
  <br>
 <p align="justify"> 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Evaluate how these outliers might affect analysis. In sales data, outliers may represent data errors. <br>
  
 <p align="center">
 <img src= "https://github.com/user-attachments/assets/12bdcada-33f3-4272-955e-9446a41003a6"style= "height: 160px;">
  
<h1 align="justify">Part 2: GETTING INPUTS AND OUTPUTS</h1>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; In this part the figure shows the verifying column names to ensure correct target  variable. <br>


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **2.1 CONVERTING 'STATUS' INTO NUMERICAL DATA  FOR DEPENDENT VARIABLE SELECTION** <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; When estimating the likelihood that an order will be completed or the elements that lead to fulfillment delays, it is best to use 'STATUS' as a dependent variable. Otherwise, concentrating on a regression technique would be more suitable if your objective is to forecast numerical results such as 'SALES'. <br>

<p align="center">
 <img src= "https://github.com/user-attachments/assets/d8dbdd4e-6076-47b6-a34f-b24d06c6a8d4" style= "height: 100px;"> <br>
 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **2.2 INDEPENDENT VARIABLE** <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; In this section, the figure shows the independent variable in the sales data is "SALES"<br>

<p align="center">
 <img src= "https://github.com/user-attachments/assets/932fd4de-c040-434b-a4ad-09ac3cb8ddf6" style= "height: 108px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **2.3 DEPENDENT VARIABLE** <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; In this section, the figure shows the dependent variable in the sales data are "'QUANTITYORDERED', 'PRICEEACH', 'MSRP','STATUS'"<br>

<p align="center">
 <img src= "https://github.com/user-attachments/assets/9fac7e2e-a168-4989-9660-431b2270292d" style= "height: 2980px;"> <br>
 
<h1 align="justify">Part 3: CREATING TRAINING SET AND THE TEST SET</h1>

<p align="center">
 <img src= "https://github.com/user-attachments/assets/9f64c35d-2b6e-4811-a37c-3dd8121d3696" style= "height: 200px;"> <br>
 
 + X_train
<p align="center">
<img src= "https://github.com/user-attachments/assets/c5a0cd67-efbf-4281-b01e-f893d2e25b52" style= "height: 200px;"> <br>

 + X_test
<p align="center">
<img src= "https://github.com/user-attachments/assets/f784f99b-2dac-4ce2-9439-70b89ec68078" style= "height: 200px;"> <br>

 + y_train
<p align="center">
<img src= "https://github.com/user-attachments/assets/3641533e-f298-475b-8cbf-b30acc6d7cc2" style= "height: 200px;"> <br>

 + y_test
<p align="center">
<img src= "https://github.com/user-attachments/assets/40ea9968-a0d3-435a-894c-0eb2147fa218" style= "height: 200px;"> <br>

<h1 align="justify">Part 4: BUILDING AND TRAINING THE MODEL</h1>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Converting historical data into actionable insights through model training can lead to better, more strategic decisions and better results. <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **4.1 BUILDING THE MODEL** <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/49494629-4530-449c-8fcb-b4bdc8469047" style= "height: 200px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **4.2 TRAINING THE MODEL** <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/0acd39d8-cd44-4006-87a8-28555c7ab846" style= "height: 200px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **4.2 INFERENCE** <br>
+ y_pred
<p align="center">
<img src= "https://github.com/user-attachments/assets/dce28f48-44ad-4dbc-8842-bef17db417dc" style= "height: 200px;"> <br>
+ y_pred
<p align="center">
<img src= "https://github.com/user-attachments/assets/7e242cca-4fb5-4e5a-a87b-5dbe8b0862fe" style= "height: 200px;"> <br>


 
<h1 align="justify">Part 5: EVALUATING THE MODEL</h1>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **5.1 R^2** <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Indicates the proportion of variance in the dependent variable explained by the independent variables. R² ranges from 0 to 1, where values closer to 1 represent a better fit. <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/5e79d89f-8583-47df-ba33-8686e059cc0e" style= "height: 200px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **5.2 ADJUSTED R^2** <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Adjusted R^2 is a modified version of R-squared that accounts for the number of predictors in a regression model. It’s useful because it penalizes the addition of irrelevant variables, helping to determine if adding more features improves the model's performance. <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/7f67f853-39a9-4df2-ba0c-25094e9bf842" style= "height: 200px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **5.3 MEAN SQUARED ERROR** <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Measures the average of the squared differences between predicted and actual values.<br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/d9f91806-fca4-4477-b500-47b9709d6f8d" style= "height: 200px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **5.4 GETTING THE COEFFICIENTS** <br> 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Interpret coefficients to understand the significance of each variable in predicting sales. <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/c2519f45-9ccb-4069-a7c5-9402dadddb08" style= "height: 200px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **5.5 VISUALIZATION** <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/de417078-f00e-4c51-9e6a-44d239dd919e" style= "height: 200px;"> <br>





<h1 align="center">LOGISTIC REGRESSION: BREAST CANCER WISCONSIN</h1>

<h1 align="justify">Part 1: Data Processing</h1>
<p align="center">
 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **1.1 IMPORTING THE DATASET** <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/6d1a4bb1-75c1-4c13-81f1-6f99142bd154" style= "height: 140px;"> <br>
<img src= "https://github.com/user-attachments/assets/33541857-1394-4831-b906-e57aa9b2f0a6" style= "height: 300px;"> <br>
<img src= "https://github.com/user-attachments/assets/6d1a4bb1-75c1-4c13-81f1-6f99142bd154" style= "height: 139px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **1.2 UNECESSARY COLUMNS** <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/100abfa0-5bbf-419f-8d42-2b270edca74c" style= "height: 57px;"> <br>
 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **1.3 CHECKING NULL VALUES** <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/312626d1-f317-4cc1-adc9-335203567c52" style= "height: 380px;"> <br>
 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **1.4 CONVERT INDEPENDENT VARIABLE COLUMN TO NUMERICAL** <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/2b572966-ff81-4d9a-a298-bcc3f5c85e62" style= "height: 298px;"> <br>
<img src= "https://github.com/user-attachments/assets/66eba55b-7332-4014-a67d-b3f3990280b6" style= "height: 290px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **1.5 GETTING THE INPUT AND OUTPUT** <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; X <br>
 
<p align="center">
<img src= "https://github.com/user-attachments/assets/dee26b14-24ca-48d3-a4a7-86007447c33f" style= "height: 298px;"> <br>
<img src= "https://github.com/user-attachments/assets/da77622a-c1de-4435-9a77-3f79e4c37cca" style= "height: 320px;"> <br>
<img src= "https://github.com/user-attachments/assets/870bbc66-4c5c-4a8d-a689-b6a7e4373564" style= "height: 325px;"> <br>
 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Y <br>
 
<p align="center">
<img src= "https://github.com/user-attachments/assets/3c1e1369-ef4a-411a-9c0a-dd1617f1815b" style= "height: 165px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **1.6 CREATING THE TRAINING SET AND THE TEST SET** <br>

<p align="center">
<img src= "https://github.com/user-attachments/assets/a8b9b20a-31a2-4130-b3d8-704d8342fb39" style= "height: 40px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;X_train <br> 

<p align="center">
<img src= "https://github.com/user-attachments/assets/f8e9d817-aa99-4175-80fa-4a7f7e5cc011" style= "height: 250px;"> <br>
<img src= "https://github.com/user-attachments/assets/e63a1295-c086-4e7a-9df5-c60f27b20da1" style= "height: 256px;"> <br>
<img src= "https://github.com/user-attachments/assets/068eaa76-48cd-4e87-8aca-3d84e616e600" style= "height: 250px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  X_test <br> 

<p align="center">
<img src= "https://github.com/user-attachments/assets/9c849718-11f3-415d-ad38-9765e94cf5f6" style= "height: 250px;"> <br>
<img src= "https://github.com/user-attachments/assets/266231a2-617b-4365-8019-c95a50717843" style= "height: 255px;"> <br>
<img src= "https://github.com/user-attachments/assets/6d00a6e5-1f4d-4ba7-8d2f-2d031035fb33" style= "height: 250px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Y_test <br> 

<p align="center">
<img src= "https://github.com/user-attachments/assets/ac1138aa-0b80-436d-bedb-df731295ab61" style= "height: 160px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Y_test <br> 

<p align="center">
<img src= "https://github.com/user-attachments/assets/2d016924-44f4-4a15-a4f3-0acaa9eefd7a" style= "height: 160px;"> <br>

<h1 align="justify">Part 2:BUILDING AND TRAINING MODEL </h1> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **2.1  BUILDING THE MODEL** <br>

<p align="center">
<img src= "https://github.com/user-attachments/assets/f05dbc07-4365-4921-9b02-dde1ac2c4f81" style= "height: 55px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **2.2  TRAIN THE MODEL** <br>

<p align="center">
<img src= "https://github.com/user-attachments/assets/477dcfe3-5b53-4d00-bb66-bfdc0907f128" style= "height: 95px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **2.3 INFERENCE**

<p align="justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;Making the predictions of the data points in the test set. <br>

<p align="center">
<img src= "https://github.com/user-attachments/assets/e89f2db1-1165-4fbf-a1a5-309490325ad7" style= "height: 45px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; y_pred <br> 

<p align="center">
<img src= "https://github.com/user-attachments/assets/726a0c3e-2679-46a1-a9d0-8b518dbb2ade" style= "height: 92px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; y_test <br> 

<p align="center">
<img src= "https://github.com/user-attachments/assets/94e2a78b-b338-4ae3-a432-2c83f984ceae" style= "height: 150px;"> <br>

<h1 align="justify">Part 3:EVALUATING THE MODEL </h1> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **3.1 CONFUSION MATRIX**

<p align="center">
<img src="https://github.com/user-attachments/assets/28d406db-c931-46e1-8609-b599be456836 "style= "height: 68px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **3.2 ACCURACY**

<p align="center">
<img src="https://github.com/user-attachments/assets/e8a91bcc-6559-4032-ad9d-e41f525c2667"style= "height: 90px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **3.3 PLOT CONFUSION MATRICES**

<p align="center">
<img src="https://github.com/user-attachments/assets/3a57e854-83ca-4220-8bdc-05bcd24f0393"style= "height: 300px;"> <br>

# V. SUMMARY AND FINDINGS
 <h1 align="center">LINEAR REGRESSION: SALES DATA</h1>

 <h1 align="center">LOGISTIC REGRESSION: BREAST CANCER WISCONSIN</h1>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **INFERENCE**

<p align="justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; The variable y_pred is the output from this model, representing predictions on the test dataset.Y_pred is to indicate whether each test sample is classified as benign (0) or malignant (1). <br>

<p align="center">
<img src="https://github.com/user-attachments/assets/f0d9cd18-9f0c-4c2a-a0f9-77902dca24e4"style= "height: 100px;"> <br>
 
<p align="justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; The y_test contains the true diagnostic classifications for each sample in the test set, identifying whether each case of breast cancer is benign (0) or malignant (1). <br>

 <p align="center">
<img src= "https://github.com/user-attachments/assets/94e2a78b-b338-4ae3-a432-2c83f984ceae" style= "height: 150px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **CONFUSION MATRIX** <br> 

<p align="justify">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  The figure attached represents the model's performance between two classes: benign (0) and malignant (1).

 + **TRUE NEGATIVE (TN)** - label 0, predicted 0 the result value is 70. This indicates that the model correctly classified 70 benign cases as benign.
 + **FALSE POSITIVE (FP)** - label 0, predicted 1 the result value is 1.This represents a single benign case that was incorrectly classified as malignantThis is known as a Type I error.
 + **FALSE NEGATIVE (FN)** - label 1, predicted 0 the result value is 0 the result value is 2.ndicating that 2 malignant cases were incorrectly classified as benign. This is known as a Type II error.
 + **TRUE POSITIVE (TP)** - label 1, predicted 1 the result value is 41 means that the model correctly classified 41 malignant cases as malignant.

  <p align="center">
<img src= "https://github.com/user-attachments/assets/6a8f65f3-599c-479a-8061-8420826f34d7"style= "height: 300px;"> <br>

# VI. REFERENCES

 + SALES DATA LINK: https://www.kaggle.com/datasets/kyanyoga/sample-sales-data 
 + BREAST CANCER WISCONSIN: https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data 




