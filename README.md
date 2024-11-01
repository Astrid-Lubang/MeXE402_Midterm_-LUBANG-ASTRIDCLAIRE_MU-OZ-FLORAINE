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
 <img src= "https://github.com/user-attachments/assets/12bdcada-33f3-4272-955e-9446a41003a6"style= "height: 200px;">
  
<h1 align="justify">Part 2: GETTING INPUTS AND OUTPUTS</h1>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; In this part the figure shows the verifying column names to ensure correct target  variable. <br>


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **2.1 CONVERTING 'STATUS' INTO NUMERICAL DATA  FOR DEPENDENT VARIABLE SELECTION** <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; When estimating the likelihood that an order will be completed or the elements that lead to fulfillment delays, it is best to use 'STATUS' as a dependent variable. Otherwise, concentrating on a regression technique would be more suitable if your objective is to forecast numerical results such as 'SALES'. <br>

<p align="center">
 <img src= "https://github.com/user-attachments/assets/d8dbdd4e-6076-47b6-a34f-b24d06c6a8d4" style= "height: 400px;"> <br>
 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **2.2 INDEPENDENT VARIABLE** <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; In this section, the figure shows the independent variable in the sales data is "SALES"<br>

<p align="center">
 <img src= "https://github.com/user-attachments/assets/932fd4de-c040-434b-a4ad-09ac3cb8ddf6" style= "height: 250px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **2.3 DEPENDENT VARIABLE** <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; In this section, the figure shows the dependent variable in the sales data are "'QUANTITYORDERED', 'PRICEEACH', 'MSRP','STATUS'"<br>

<p align="center">
 <img src= "https://github.com/user-attachments/assets/9fac7e2e-a168-4989-9660-431b2270292d" style= "height: 250px;"> <br>
 
<h1 align="justify">Part 3: CREATING TRAINING SET AND THE TEST SET</h1>

<p align="center">
 <img src= "https://github.com/user-attachments/assets/9f64c35d-2b6e-4811-a37c-3dd8121d3696" style= "height: 170px;"> <br>
 
 + X_train
<p align="center">
<img src= "https://github.com/user-attachments/assets/c5a0cd67-efbf-4281-b01e-f893d2e25b52" style= "height: 250px;"> <br>

 + X_test
<p align="center">
<img src= "https://github.com/user-attachments/assets/f784f99b-2dac-4ce2-9439-70b89ec68078" style= "height: 250px;"> <br>

 + y_train
<p align="center">
<img src= "https://github.com/user-attachments/assets/3641533e-f298-475b-8cbf-b30acc6d7cc2" style= "height: 190px;"> <br>

 + y_test
<p align="center">
<img src= "https://github.com/user-attachments/assets/40ea9968-a0d3-435a-894c-0eb2147fa218" style= "height: 190px;"> <br>

<h1 align="justify">Part 4: BUILDING AND TRAINING THE MODEL</h1>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Converting historical data into actionable insights through model training can lead to better, more strategic decisions and better results. <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **4.1 BUILDING THE MODEL** <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/49494629-4530-449c-8fcb-b4bdc8469047" style= "height: 100px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **4.2 TRAINING THE MODEL** <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/0acd39d8-cd44-4006-87a8-28555c7ab846" style= "height: 250px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **4.2 INFERENCE** <br>
+ y_pred
<p align="center">
<img src= "https://github.com/user-attachments/assets/dce28f48-44ad-4dbc-8842-bef17db417dc" style= "height: 400px;"> <br>
 
+ y_test
<p align="center">
<img src= "https://github.com/user-attachments/assets/7e242cca-4fb5-4e5a-a87b-5dbe8b0862fe" style= "height: 220px;"> <br>


 
<h1 align="justify">Part 5: EVALUATING THE MODEL</h1>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **5.1 R^2** <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Indicates the proportion of variance in the dependent variable explained by the independent variables. R² ranges from 0 to 1, where values closer to 1 represent a better fit. <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/5e79d89f-8583-47df-ba33-8686e059cc0e" style= "height: 100px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **5.2 ADJUSTED R^2** <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Adjusted R^2 is a modified version of R-squared that accounts for the number of predictors in a regression model. It’s useful because it penalizes the addition of irrelevant variables, helping to determine if adding more features improves the model's performance. <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/7f67f853-39a9-4df2-ba0c-25094e9bf842" style= "height: 300px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **5.3 MEAN SQUARED ERROR** <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Measures the average of the squared differences between predicted and actual values.<br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/d9f91806-fca4-4477-b500-47b9709d6f8d" style= "height: 140px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **5.4 GETTING THE COEFFICIENTS** <br> 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Interpret coefficients to understand the significance of each variable in predicting sales. <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/c2519f45-9ccb-4069-a7c5-9402dadddb08" style= "height: 200px;"> <br>


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **5.5 VISUALIZATION** <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/ea745008-c9d6-4ce5-95cb-422c4aaf257e" style= "height: 150px;"> <br>
<img src= "https://github.com/user-attachments/assets/85518857-fe07-4555-a212-a81a1e2a3605" style= "height: 500px;"> <br>




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
<img src= "https://github.com/user-attachments/assets/3a9107aa-926b-457a-b5c9-7d95bdaacf0a" style= "height: 165px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **1.6 CREATING THE TRAINING SET AND THE TEST SET** <br>

<p align="center">
<img src= "https://github.com/user-attachments/assets/19b1559e-ef14-4d81-a670-02928d35b329" style= "height: 150px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;X_test <br> 

<p align="center">
<img src= "https://github.com/user-attachments/assets/2a491adc-52a4-4dee-a5e0-4fdc73a67afb" style= "height: 250px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  X_train <br> 

<p align="center">
<img src= "https://github.com/user-attachments/assets/7f68b08a-9342-4db0-a373-7fb6fc0d318b" style= "height: 250px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Y_test <br> 

<p align="center">
<img src= "https://github.com/user-attachments/assets/2278cee3-59d1-4da5-9e51-b4151765ff2d" style= "height: 160px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Y_train <br> 

<p align="center">
<img src= "https://github.com/user-attachments/assets/53c3ed38-2bca-4817-a830-65db511a2521" style= "height: 160px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **1.7 FEATURE SCALING** <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/b197727a-606b-433e-a241-bee16a8584e4" style= "height: 400px;"> <br>

 
<h1 align="justify">Part 2:BUILDING AND TRAINING MODEL </h1> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **2.1  BUILDING THE MODEL** <br>

<p align="center">
<img src= "https://github.com/user-attachments/assets/5a6e6fa0-670e-41ce-b148-ec6a60eea26a" style= "height: 80px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **2.2  TRAIN THE MODEL** <br>

<p align="center">
<img src= "https://github.com/user-attachments/assets/7a7a077d-bb05-4bd1-aa60-de9a652405fe" style= "height: 105px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **2.3 INFERENCE**

<p align="justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;Making the predictions of the data points in the test set. <br>

<p align="center">
<img src= "https://github.com/user-attachments/assets/7fd26daf-df25-41e5-8f96-d8098433aeaa" style= "height: 105px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; y_pred <br> 

<p align="center">
<img src= "https://github.com/user-attachments/assets/38b160fd-61d7-4e2a-b91e-0e8cd11a704a" style= "height: 92px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; y_test <br> 

<p align="center">
<img src= "https://github.com/user-attachments/assets/9ebd17c9-7a7d-4781-9d1c-35da49278705" style= "height: 150px;"> <br>

<h1 align="justify">Part 3:EVALUATING THE MODEL </h1> 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **3.1 CONFUSION MATRIX**

<p align="center">
<img src="https://github.com/user-attachments/assets/aa09cde9-9af1-45f9-b1f3-8dc3a8fe25d6"style= "height: 175px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **3.2 ACCURACY**

<p align="center">
<img src="https://github.com/user-attachments/assets/58022033-41fa-457e-91b2-6e4089e28143"style= "height: 175px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **3.3 PLOT CONFUSION MATRICES**

<p align="center">
<img src="https://github.com/user-attachments/assets/cfecdc17-4655-44d7-916a-e395225f875c"style= "height: 400px;"> <br>

# V. SUMMARY AND FINDINGS
 <h1 align="center">LINEAR REGRESSION: SALES DATA</h1>
 
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Explain the significance of coefficients and the model's predictive power**
 
 <p align="center">
<img src="https://github.com/user-attachments/assets/e979e0ae-86b7-4f80-bdc4-ff0eb9ec8f8b"style= "height: 300px;"> <br>

 <h1 align="center">LOGISTIC REGRESSION: BREAST CANCER WISCONSIN</h1>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **INFERENCE**

<p align="justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; The variable y_pred is the output from this model, representing predictions on the test dataset.Y_pred is to indicate whether each test sample is classified as benign (0) or malignant (1). <br>

<p align="center">
<img src="https://github.com/user-attachments/assets/4a03d810-9794-462d-9a33-771145b918a6"style= "height: 180px;"> <br>
 
<p align="justify">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; The y_test contains the true diagnostic classifications for each sample in the test set, identifying whether each case of breast cancer is benign (0) or malignant (1). <br>

 <p align="center">
<img src= "https://github.com/user-attachments/assets/ca7b233f-e209-4876-bf9b-f0cf77735f97" style= "height: 190px;"> <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **CONFUSION MATRIX** <br> 

<p align="justify">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  The figure attached represents the model's performance between two classes: benign (0) and malignant (1).

 + **TRUE NEGATIVE (TN)** - label 0, predicted 0 the result value is 65. This indicates that the model correctly classified 70 benign cases as benign.
 + **FALSE POSITIVE (FP)** - label 0, predicted 1 the result value is 2.This represents a single benign case that was incorrectly classified as malignantThis is known as a Type I error.
 + **FALSE NEGATIVE (FN)** - label 1, predicted 0 the result value is 2 the result value is 2.ndicating that 2 malignant cases were incorrectly classified as benign. This is known as a Type II error.
 + **TRUE POSITIVE (TP)** - label 1, predicted 1 the result value is 44 means that the model correctly classified 41 malignant cases as malignant.

  <p align="center">
<img src= "https://github.com/user-attachments/assets/8f98cf65-4d0a-419b-bff9-4d62dcde6348"style= "height: 300px;"> <br>

# VI. REFERENCES

 + SALES DATA LINK: https://www.kaggle.com/datasets/kyanyoga/sample-sales-data 
 + BREAST CANCER WISCONSIN: https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data 




