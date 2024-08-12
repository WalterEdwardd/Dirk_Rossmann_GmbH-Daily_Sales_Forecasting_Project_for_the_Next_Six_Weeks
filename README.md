# Dirk Rossmann GmbH - Forecast The Daily Sales For The Next Six Weeks Project
A project aimed at processing, exploring and forecasting daily sales data for Dirk Rossmann GmbH for the next six weeks.

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
2.	To build models able to predict sales based on stores and sales history features
3.	To analyze and compare models performance in order to choose the best model

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
git clone https://github.com/WalterEdwardd/Dirk_Rossmann_GmbH-Forecast_The_Daily_Sales_For_The_Next_Six_Weks_Project.git

### 2. Requirements
List of libraries:
-	pip install pandas
-	pip install numpy
-	pip install seaborn
-	pip install matplotlib
-	pip install scikit-learn 
-	pip install xgboost
-	pip install lightgbm
-	pip install pickle
-	pip install tensorflow
-	pip install keras

## III. Usage
Run the main script to start prediction: [file]("Resources/Code/DIRKRO~1.IPY")
## IV. Data
This data has been provided by the Rossman company and used within the provided rules on their Kaggle competition page for an exploratory analysis (Rossmann Store Sales, 2015). The data is provided in two tables, stores and train.
- The store table contains the metadata for every single store including the following:
1. Store - an ID that represents the store
2. StoreType - differentiates between 4 different store models: A, B, C, D
3. Assortment - describes an assortment level: A = Basic, B = Extra, C = Extended
4. CompetitionDistance - describes the distance in meters to the nearest competitor store
5. CompetitionOpenSinceMonth - gives the approximate month of the time the nearest competitor was opened
6. CompetitionOpenSinceYear - gives the approximate year of the time the nearest competitor was opened
7. Promo2 - Promo2 is a continuing and consecutive promotion for some stores: 0 = store is not participating, 1 = store is participating
8. Promo2SinceWeek - describes the calendar week when the store started participating in Promo
9. Promo2SinceYear - describes the year when the store started participating in Promo
10. PromoInterval - describes the consecutive intervals Promo2 is started, naming the months the promotion is started anew. E.g. "Feb, May, Aug, Nov" means each round starts in February, May, August, November of any given year for that store

- The sales table contains the sales data for individual stores at a daily level along with the details about the day:
1. Store - a unique ID for each store
2. DayOfWeek - Describes the day of the week (1-Monday till 7-Sunday)
3. Date - Describes the date on the day
4. Sales - the turnover for any given day ($) (this is what you are forecasting)
5. NumberOfCustomers - the number of customers on a given day
6. Open - an indicator for whether the store was open: 0 = closed, 1 = open
7. Promo - indicates whether a store is running a promo on that day
8. StateHoliday - indicates a state holiday. Normally all stores, with few exceptions, are closed on state holidays. Note that all schools are closed on public holidays and weekends. A = public holiday, B = Easter holiday, C = Christmas, D = None
9. SchoolHoliday - indicates if the (Store, Date) was affected by the closure of public schools: 0 = not affected, 1 = affected

## V. Results
### 1. Random Forest Regressor
#### a. Define
![image](https://github.com/user-attachments/assets/63f96a4a-0e41-4567-bca0-cb3d3025186a)
#### b. HyperParameters Tuning
![image](https://github.com/user-attachments/assets/a514a147-66bf-4cc7-9e3b-c9846cb35bfc)
#### c.Training and Evaluating Model
![image](https://github.com/user-attachments/assets/1ebd5bd6-ecdd-454a-a691-a955a1e1ca58)
#### d. Features Importance
![image](https://github.com/user-attachments/assets/404fd6c1-c9ae-4685-9241-24dee739dfb6)

### 2. XGBoost Regressor
#### a. Define
![image](https://github.com/user-attachments/assets/8106a4c6-d320-474b-8905-f2a9a6ffd68d)
#### b. HyperParameters Tuning
![image](https://github.com/user-attachments/assets/c64f8241-663f-4134-a489-3f710c003113)
#### c.Training and Evaluating Model
![image](https://github.com/user-attachments/assets/46ef4451-a13a-4117-a65b-bc1f67a5cc91)
#### d. Features Importance
![image](https://github.com/user-attachments/assets/ef74c888-987c-4c43-aa96-62a7ff23f266)

### 3. LightGBM Regressor
#### a. Define
![image](https://github.com/user-attachments/assets/b8155a9b-a25e-4469-a5c8-ff9ce671a53d)
#### b. HyperParameters Tuning
![image](https://github.com/user-attachments/assets/aabe1da1-9659-4030-a198-716ff3338525)
#### c.Training and Evaluating Model
![image](https://github.com/user-attachments/assets/9da95f1d-9bf7-40f5-982a-404ac35d0b3f)
#### d. Features Importance
![image](https://github.com/user-attachments/assets/76f1cae5-d7e4-4288-8f6a-de916a3e3b16)

### 4. Long Short-Term Memory
#### a. Define
![image](https://github.com/user-attachments/assets/3d34c443-2438-4b96-a31e-72251d89bd8b)
#### b. Build the Model
![image](https://github.com/user-attachments/assets/f267fbfb-357c-4c6d-9804-bcadc3cdc4ec)
#### c.Training and Evaluating Model
![image](https://github.com/user-attachments/assets/9abfa2be-3ec5-4f3c-8e50-ed7d5a91200a)

### 5. Comparating Model
![image](https://github.com/user-attachments/assets/b2d3d329-3a87-45b9-83f7-eec84bc04860)

### 6. Visualization The Daily Sales
#### Store 1
![image](https://github.com/user-attachments/assets/2be574f8-e3fc-4f0f-ba6d-1429f8d66f11)
#### Store 3
![image](https://github.com/user-attachments/assets/623cc264-6e2d-4f1d-ac80-488b2b6f88d3)
#### Store 8
![image](https://github.com/user-attachments/assets/f6881b91-fc9f-4816-b651-a35d611f9aba)
#### Store 9
![image](https://github.com/user-attachments/assets/1be5af60-235a-41d0-945d-8e15ac5daf28)
#### Store 13
![image](https://github.com/user-attachments/assets/630e70fc-0ab4-42c8-a0d4-cc234b5ee910)
#### Store 25
![image](https://github.com/user-attachments/assets/98a04294-1cce-4063-81ac-11aee1514059)
#### Store 29
![image](https://github.com/user-attachments/assets/a7751063-3b1b-434b-b5fd-4d203f99ecff)
#### Store 31
![image](https://github.com/user-attachments/assets/327754d1-143e-4153-af14-18e8433f9d3a)
#### Store 46
![image](https://github.com/user-attachments/assets/f4733820-74a8-4671-a0fa-40f0836a8d06)

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
