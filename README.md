# Dirk Rossmann GmbH - Forecast The Daily Sales For The Next Six Weeks_Python_Project
A project aimed at forecasting daily sales data for Dirk Rossmann GmbH for the next six weeks.

Tools used: Python, Excel, PowerPoint

## I. Description
This project involves analyzing sales data for Dirk Rossmann GmbH to forecast daily sales for the next six weeks.

### 1. Problem Statement
Rossmann is a European drug distributor which operates over 3,000 drug stores across seven European countries. Since a lot of drugs come with a short shelf life, that is, they do not have a long expiry date, it becomes imperative for Rossmann to accurately forecast sales at their individual stores. Currently, the forecasting is taken care of by the store managers who are tasked with forecasting daily sales for the next six weeks.
As expected, store sales are influenced by many factors, including promotional campaigns, competition, state holidays, seasonality, and locality.
With thousands of individual managers predicting sales based on their unique circumstances and intuitions, the accuracy of the forecasts is quite varied. To overcome this problem, the company has decided to build a forecasting model to forecast the daily sales for the next six weeks.
Note - Since the company is just embarking on this project, the scope has been kept to nine key stores across Europe. The stores are key for the company keeping in mind the revenue and historical prestige associated with them. These stores are numbered - 1, 3, 8, 9, 13, 25, 29, 31 and 46.

### 2. Goals of the Study
The main objectives of this case study are as follows:
1.	To apply data preprocessing and preparation techniques in order to obtain clean data (EDA)
2.	To build a suitable model able to predict sales based on stores and sales history features
3.	To develop deeper data analysis capabilitie.

### 3. Ethical Considerations:
This data has been provided by the Rossman company and used within the provided rules on their Kaggle competition page for an exploratory analysis (Rossmann Store Sales, 2015). There is no personal identifiable information (PII) in this data set.

### 4. Table of Contents
- Introduction:
  - Problem Statement
  - Goals of the Study
  - Ethical Considerations
  - Variable Explanation

- Data Understanding
  - Data Pre-Processing:
    - Raw Data Processing
    - Merging of Data Sources
    - Outlier Processing

- Exploratory Data Analyst (EDA):
  - Sales Analysis
  - Number of Customers Analysis
  - Average Sales per Transactions and Others Analysis
  - Summary Insights
  - Correlation Check
  - Label Encoding for Each Object Data Type

- Machine Learning
  - Preparing for Machine Learning
  - Machine Learning Model:
  - Random Forest Regressor
  - XGBoost Regressor
  - Light GBM Regressor

- Deep Learning
  - Preparing for Deep Learning
  - Deep Learning Model:
  - Long Short Term Memory (LSTM)

- Comparison and Evaluation Models
  - R2
  - Mean Absolute Error
  - Mean Square Error
  - Root Mean Square Error

- Forecasting
  - Preparing for Forecasting
  - Predicting Future Daily Sales
  - Visualization Future Daily Sales

## II. Installation
To get started with this project, clone the repository and install the required Python packages

### 1. Clone repository
git clone [link](https://github.com/WalterEdwardd/Dirk_Rossmann_GmbH-Forecast_The_Daily_Sales_For_The_Next_Six_Weks_Project.git)

### 2. Requirements
List of libraries:
-	[pip install pandas](https://pypi.org/project/pandas/)
-	[pip install numpy](https://pypi.org/project/numpy/)
-	[pip install seaborn](https://pypi.org/project/seaborn/)
-	[pip install matplotlib](https://pypi.org/project/matplotlib/)
-	[pip install scikit-learn](https://pypi.org/project/scikit-learn/)
-	[pip install xgboost](https://pypi.org/project/xgboost/)
-	[pip install lightgbm](https://pypi.org/project/lightgbm/)
-	[pip install pickle](https://pypi.org/project/pickle5/)
-	[pip install tensorflow](https://pypi.org/project/tensorflow/)
-	[pip install keras](https://pypi.org/project/keras/)

## III. Usage
Run the main script to start prediction: [Jupyter Notebook File](Resources/Code/DIRKRO~1.IPY)

## IV. Data
This data has been provided by the Rossman company and used within the provided rules on their Kaggle competition page for an exploratory analysis (Rossmann Store Sales, 2015). The data is provided in 2 CSV files:
- [store file](Resources/Data)
- [sales file](Resources/Data)

[Details here](Resources/Data/Dataset_Description.txt)

## V. Results
### 1. Random Forest Regressor
#### a. Define
![image](https://github.com/user-attachments/assets/9d64ce4a-e850-45fb-875e-c703869f54af)
#### b. HyperParameters Tuning
![image](https://github.com/user-attachments/assets/1172242e-b0bd-41b8-90f9-637d224076ba)
#### c.Training and Evaluating Model
![image](https://github.com/user-attachments/assets/a5afa06d-d429-4db1-bd06-4b3329735fb2)
#### d. Features Importance
![image](https://github.com/user-attachments/assets/05b8a73e-00b5-4c0e-a22d-fd53e1f4594a)

### 2. XGBoost Regressor
#### a. Define
![image](https://github.com/user-attachments/assets/f0936ec4-9969-41bc-9630-e7b8f082e894)
#### b. HyperParameters Tuning
![image](https://github.com/user-attachments/assets/a6dbc1d2-b1f3-41ac-926c-c18aca2c4dd7)
#### c.Training and Evaluating Model
![image](https://github.com/user-attachments/assets/ba99285c-c0b6-4950-80af-518aef04bdf0)
#### d. Features Importance
![image](https://github.com/user-attachments/assets/3a553726-f2e3-4707-b219-13ef7f0f3ef8)

### 3. LightGBM Regressor
#### a. Define
![image](https://github.com/user-attachments/assets/85414bc3-b237-4627-acf9-3d4e084e9494)
#### b. HyperParameters Tuning
![image](https://github.com/user-attachments/assets/44a2eed5-018f-4a25-b56f-6e385c655894)
#### c.Training and Evaluating Model
![image](https://github.com/user-attachments/assets/9e2953cc-ca5e-426c-b7ff-c8de8a8ce702)
#### d. Features Importance
![image](https://github.com/user-attachments/assets/47ed41d5-0928-43da-bf8b-22c044c4753c)

### 4. Long Short-Term Memory
#### a. Define
![image](https://github.com/user-attachments/assets/52162b1a-6e1c-490d-ae3a-12fdea0a0e8e)
#### b. Build the Model
![image](https://github.com/user-attachments/assets/ffa90a6c-92ac-4ec2-bf84-e2c0b514b465)
#### c.Training and Evaluating Model
![image](https://github.com/user-attachments/assets/16d70aec-1af8-4dd2-bd11-29283076046f)

### 5. Comparating Model
![image](https://github.com/user-attachments/assets/be7fcd3d-f166-4994-840b-a6ec10a40f13)

### 6. Visualization The Daily Sales
#### Store 1
![image](https://github.com/user-attachments/assets/dd98efac-98d4-4f38-8f7a-311c2514057a)
#### Store 3
![image](https://github.com/user-attachments/assets/5b4ce91f-dc1b-4f91-81be-44b3ffec4b1f)
#### Store 8
![image](https://github.com/user-attachments/assets/85ddc162-c458-4497-bab0-3d581d1270a3)
#### Store 9
![image](https://github.com/user-attachments/assets/0c60ae46-2795-4706-9c10-15c7a55e7b42)
#### Store 13
![image](https://github.com/user-attachments/assets/234c980f-6733-4f2e-b308-43d43ee97ddf)
#### Store 25
![image](https://github.com/user-attachments/assets/e26b096a-b6c4-4be1-ae85-9b2cab0321c5)
#### Store 29
![image](https://github.com/user-attachments/assets/ce5065f7-2fa3-43b1-bf0e-4a3e513b78ab)
#### Store 31
![image](https://github.com/user-attachments/assets/1345a87e-dd6c-43ff-9c1b-f3202a9c4a0b)
#### Store 46
![image](https://github.com/user-attachments/assets/56a2b189-e31b-4670-96a3-50e8bc7d3bcf)

### 7. Suggestion
![image](https://github.com/user-attachments/assets/53b0939e-1031-4f09-bb28-ee48af4cb1c0)

## VI. Contributing
Contributions are welcome! Please submit a pull request or open an issue for any suggestions or improvements.
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## VII. Author
Created by [Nhu Dai Tran](https://github.com/WalterEdwardd)

<img src="https://github.com/user-attachments/assets/01b769fa-5c75-44db-819f-3fc8781c7e98" alt="Description" width="300" height="400">
