# TABLE OF CONTENTS
  * [I. INTRODUCTION](#i-introduction)
  * [II. DATASET DESCRIPTION](#ii-datasetdescription)
  * [III. PROJECT OBJECTIVES](#iii-projectobjectives)
  * [IV. DOCUMENTATION](#iv-documentation) <br>
      + [GRABENG README TO METHODOLOGY](methodology)
    
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
<img src= "https://github.com/user-attachments/assets/39e5d729-37f2-4cb1-9f45-67807fe53130" style= "height: 127px;"> 
<img src= "https://github.com/user-attachments/assets/6c020d51-4c15-453f-a44f-b64166210dda" style="height: 300px;"> 
<img src= "https://github.com/user-attachments/assets/38311bef-64e9-4ae8-b568-ffc33cf9bc68" style="height: 268px;">
</p>
 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  **1.2 HANDLE MISSING VALUES**
  <br>
 <p align="justify"> 
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; In this part the process involves indentifying and addressing any gaps in dataset. This may include the checking missing values and dropping the missing values.The figures attached are the step by step process. <br>
  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  **Checking Missing Values** <br>
 <p align="center">
 <img src= "https://github.com/user-attachments/assets/0f1677dc-f317-4dff-b1c3-8dcf7df273ed" style= "height: 325px;"> <br>
  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  **Dropping Missing Values** <br>
<p align="center">
<img src= "https://github.com/user-attachments/assets/b07bc3cc-a12d-4b98-8fad-27fad6e602f5" style= "height: 300px;"> 
  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **1.3 CHECK FOR OUTLIERS**
  <br>
 <p align="justify"> 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Evaluate how these outliers might affect analysis. In sales data, outliers may represent data errors. <br>
  
 <p align="center">
 <img src= "https://github.com/user-attachments/assets/9f4852fe-962b-4459-a05f-04e0b177a5b2" style= "height: 100px;">
  
<h1 align="justify">Part 2: GETTING INPUTS AND OUTPUTS</h1>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; In this part the figure shows the verifying column names to ensure correct target  variable. <br>

<p align="center">
 <img src= "https://github.com/user-attachments/assets/f689442d-b6f3-4eab-9824-fa08f6f7d784" style= "height: 350px;"> <br>
 <img src= "https://github.com/user-attachments/assets/b41f675b-f238-45f4-bffd-0d5c17ab0bc7" style= "height: 335px;"> <br>
 <img src= "https://github.com/user-attachments/assets/09686667-e6d5-47c1-9f27-dd86e120f14b" style= "height: 305px;"> <br>
 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **2.1 INDEPENDENT VARIABLE** <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; In this section, the figure shows the independent variable in the sales data is "SALES"<br>

<p align="center">
 <img src= "https://github.com/user-attachments/assets/3f5ebf8c-9d5e-4155-8406-2af05d87158a" style= "height: 190px;"> <br>
 
<h1 align="justify">Part 3: CREATING TRAINING SET AND THE TEST SET</h1>
<h1 align="justify">Part 4: EVALUATING THE MODEL</h1>

<h1 align="center">LOGISTIC REGRESSION: BREAST CANCER WISCONSIN</h1>
 
 








