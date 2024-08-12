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
•	Introduction:
o	Problem Statement
o	Goals of the Study
o	Ethical Considerations
o	Variable Explanation
•	Data Understanding
•	Data Pre-Processing:
o	Raw Data Processing
o	Merging of Data Sources
o	Outlier Processing
•	Exploratory Data Analyst (EDA):
o	Sales Analysis
o	Number of Customers Analysis
o	Average Sales per Transactions and Others Analysis
o	Summary Insights
o	Correlation Check
o	Label Encoding for Each Object Data Type
•	Machine Learning
o	Preparing for Machine Learning
o	Machine Learning Model:
	Random Forest Regressor
	XGBoost Regressor
	Light GBM Regressor
•	Deep Learning
o	Preparing for Deep Learning
o	Deep Learning Model:
	Long Short Term Memory (LSTM)
•	Comparison and Evaluation Models
o	R2
o	Mean Absolute Error
o	Mean Square Error
o	Root Mean Square Error
•	Forecasting
o	Preparing for Forecasting
o	Predicting Future Daily Sales
o	Visualization Future Daily Sales

## II. Installation
To get started with this project, clone the repository and install the required Python packages
### 1. Clone repository
```bash
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
Chạy script chính để bắt đầu dự đoán:
1. **Data Preparation**: Ensure your data is in the correct format and placed in the `data/` directory.
2. **Run the Analysis**: Execute the main script to start the analysis:

## IV. Data
This data has been provided by the Rossman company and used within the provided rules on their Kaggle competition page for an exploratory analysis (Rossmann Store Sales, 2015). The data is provided in two tables, stores and train.
-The store table contains the metadata for every single store including the following:
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

-The sales table contains the sales data for individual stores at a daily level along with the details about the day:
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
-	Model and Evaluating
-	Daily sales charts

## VI. Contributing
Contributions are welcome! Please submit a pull request or open an issue for any suggestions or improvements.
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## VII. Author
Created by [Nhu Dai Tran](https://github.com/WalterEdwardd)
