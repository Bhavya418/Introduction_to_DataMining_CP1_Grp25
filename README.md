# Introduction_to_DataMining_CP1_Grp25

# **Seoul Bike Trip**
> The most basic metric for all forms of transportation is trip length. Therefore, accurate trip-time prediction is essential for the development of Intelligent Transportation Systems (ITS) and traveller information systems. In order to forecast the duration of a journey, we used certain optimized data mining techniques to forecast the duration of trips involving rental bikes in the bike-sharing programme in Seoul. The forecast is made using a combination of weather data and Pickup and Drop location data.


## Introduction

> There are 9.7 Million data instances and 26 features.
> The Data used include trip duration, trip distance, pickup-dropoff latitude and longitude, temperature, precipitation, wind speed, humidity, solar radiation, snowfall, ground temperature and 1-hour average dust concentration.
> 1. **Trip Duration**: It represents the duration of a bike trip in some unit of time, such as minutes or seconds.
> 1. **Trip Distance**: The distance covered during the bike trip, typically measured in kilometres or miles. This feature can help in understanding how to trip duration relates to the distance traveled.
> 1. **Pickup and Dropoff Latitude and Longitude**: These are geographical coordinates representing the exact location where the bike trip starts (pickup) and ends (dropoff). Latitude and longitude are used to pinpoint specific locations on the Earth's surface.
> 1. **Temperature**: The temperature at the time of the trip, usually measured in degrees Celsius or Fahrenheit. It can provide insights into how weather conditions affect trip duration.
> 1. **Precipitation**: This feature indicates whether there was any form of precipitation (rain, snow, etc.) during the trip. It's often represented as a binary variable (0 for no precipitation, 1 for precipitation).
> 1. **Wind Speed**: The speed of the wind at the time of the trip, measured in units like kilometres per hour (km/h) or meters per second (m/s). Wind speed can influence the ease of cycling.
> 1. **Humidity**: The level of moisture or humidity in the air during the trip, often represented as a percentage. High humidity can affect comfort during cycling.
> 1. **Solar Radiation**: Solar radiation measures the amount of energy received from the sun during the trip. It's typically measured in watts per square meter (W/m²) and can impact temperature and weather conditions.
> 1. **Snowfall**: Indicates whether there was snowfall during the trip, usually represented as a binary variable (0 for no snowfall, 1 for snowfall). Snowfall can significantly affect road conditions and trip duration.
> 1. **Ground Temperature**: The temperature of the ground or road surface at the time of the trip. This can be important, especially in cold or icy conditions.
> 1. **1-Hour Average Dust Concentration**: This feature represents the concentration of particulate matter (dust) in the air, typically measured in micrograms per cubic meter (µg/m³). It provides information about air quality, which can affect health and comfort during the trip.

## Data Preprocessing 
> - The first step is to check a number of null values and either replace them or remove them.
> - The second step is to remove the outliers from the dataset which are important and possibly have unwanted instances.
> - The third step is to remove the correlated features by plotting the heatmap and removing the features with a correlation greater than 80%.
>   
>  ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/36809aac-99d4-4141-8e2c-0b70c0a90bb7)

> ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/5f421047-9ee2-461b-9b44-8359c7bcc326)



## Exploratory Data Analysis
> First of all, we plotted violin plots to understand the distribution of the features.
> Then we plotted different plots to understand the relationship between different features such as linear relationships which features are more important than others.
> - The plots for the following can be found in the file.
> - Certain important plots:

>  ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/5330fd05-90dd-4e0a-8f83-07401872df7c)
  
>  ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/0b1ea625-affc-483b-b367-739075a63e0e)

>  ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/f1b801dd-32bd-4a7f-bda9-e5bfcfc8bd4c)

>  ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/ce62e1f7-f671-475e-b467-b2e9a029db03)

> ![image](https://github.com/Bhavya418/Introduction_to_DataMining_CP1_Grp25/assets/85784299/939063f4-f853-472f-ab85-36c8e502e122)

  
## Machine Learning and Data Transformations

> - We performed two data transformation techniques :
>   1. Standardization using z-score
>   2. Normalization using min-max score
>      
> Then as the dataset has been transformed and the unwanted features have been removed, we decided that we would predict the duration of the trip as that would benefit the bike rental about how to efficiently plan to provide their rides and charge accordingly. What rental companies will do is, they will have charges according to the duration it takes, the only thing the customer has to enter is the pick-up place and time along with the destination place and time, other features act as per the situation and thus give proper pricing.

> Different Models that we trained
> 1. Linear Regression
> 2. Polynomial Regression
> 3. Random Forest Regressor
> 4. Gradient Boosting Linear Regression
> 5. XGB Booster 

> - We even did some feature engineering and optimization techniques where we tried considering the weather, trained the model and obtained a good RMSE score, absolute error and accuracy.
> - We tried to plot the feature importance and found out that distance is the most important feature for estimating duration.
> - We found out that random forest regressor is the best and we implemented the ML pipeline on that.



## Course Project 02

In a credit risk analysis dataset from Kaggle, the columns and their meanings are as follows:

1. *id*: A unique identifier for each record in the dataset.
2. *member_id*: A unique identifier for each member.
3. *loan_amnt*: The requested loan amount.
4. *funded_amnt*: The actual funded amount of the loan.
5. *funded_amnt_inv*: The total amount funded by investors for the loan.
6. *term*: The term (e.g., 36 months or 60 months) of the loan.
7. *int_rate*: The interest rate on the loan.
8. *installment*: The monthly payment for the loan.
9. *grade*: The loan grade assigned by the lending platform.
10. *sub_grade*: A sub-category within the loan grade.
11. *emp_title*: The title of the borrower's employment.
12. *emp_length*: The length of time the borrower has been employed.
13. *home_ownership*: The type of home ownership (e.g., own, rent, mortgage).
14. *annual_inc*: The annual income of the borrower.
15. *verification_status*: The status of income verification for the borrower.
16. *issue_d*: The date when the loan was issued.
17. *pymnt_plan*: Whether the loan has a payment plan.
18. *desc*: A description provided by the borrower.
19. *purpose*: The purpose of the loan.
20. *title*: The title of the loan provided by the borrower.
21. *zip_code*: The borrower's zip code.
22. *addr_state*: The state where the borrower resides.
23. *dti*: The debt-to-income ratio of the borrower.
24. *delinq_2yrs*: The number of 30+ days past due in the borrower's credit report.
25. *earliest_cr_line*: The date when the borrower's earliest credit line was opened.
26. *inq_last_6mths*: The number of credit inquiries in the last 6 months.
27. *mths_since_last_delinq*: The number of months since the last delinquency.
28. *mths_since_last_record*: The number of months since the last public record.
29. *open_acc*: The number of open credit lines in the borrower's credit profile.
30. *pub_rec*: The number of public derogatory records on the borrower's credit report.
31. *revol_bal*: The borrower's revolving balance on credit cards or lines of credit.
32. *revol_util*: The borrower's revolving utilization rate.
33. *total_acc*: The total number of credit lines in the borrower's credit profile.
34. *initial_list_status*: The initial listing status of the loan.
35. *out_prncp*: The outstanding principal amount of the loan.
36. *out_prncp_inv*: The outstanding principal amount of the loan that is invested.
37. *total_pymnt*: The total amount paid by the borrower.
38. *total_pymnt_inv*: The total amount paid by the borrower's investors.
39. *total_rec_prncp*: The total principal amount received to date.
40. *total_rec_int*: The total interest amount received to date.
41. *total_rec_late_fee*: The total late fee amount received to date.
42. *recoveries*: The post-charge-off recovery amount.
43. *collection_recovery_fee*: The post-charge-off collection recovery fee.
44. *last_pymnt_d*: The date of the last payment received.
45. *last_pymnt_amnt*: The last total payment amount received.
46. *next_pymnt_d*: The date of the next payment.
47. *last_credit_pull_d*: The date when the last credit inquiry was pulled.
48. *collections_12_mths_ex_med*: The number of collections in the last 12 months excluding medical collections.
49. *mths_since_last_major_derog*: The number of months since the last major derogatory incident.
50. *policy_code*: A code related to the lending policy.
51. *application_type*: The type of loan application.
52. *annual_inc_joint*: The annual income of the borrower and co-borrower if applicable.
53. *dti_joint*: The debt-to-income ratio of the borrower and co-borrower if applicable.
54. *verification_status_joint*: The income verification status for the borrower and co-borrower if applicable.
55. *acc_now_delinq*: The number of accounts currently delinquent.
56. *tot_coll_amt*: The total collection amounts ever owed.
57. *tot_cur_bal*: The total current balance of all accounts.
58. *open_acc_6m*: The number of open credit lines in the last 6 months.
59. *open_il_6m*: The number of currently active installment trades.
60. *open_il_12m*: The number of currently active installment trades opened in the last 12 months.
61. *open_il_24m*: The number of currently active installment trades opened in the last 24 months.
62. *mths_since_rcnt_il*: The months since most recent installment accounts opened.
63. *total_bal_il*: Total current balance of all installment accounts.
64. *il_util*: Ratio of total current balance to high credit/credit limit on all install trade accounts.
65. *open_rv_12m*: The number of revolving trades opened in the last 12 months.
66. *open_rv_24m*: The number of revolving trades opened in the last 24 months.
67. *max_bal_bc*: Maximum current balance owed on all revolving accounts.
68. *all_util*: Balance to credit limit on all trades.
69. *total_rev_hi_lim*: Total revolving high credit/credit limit.
70. *inq_fi*: Number of personal finance-related inquiries.
71. *total_cu_tl*: Number of finance trades.
72. *inq_last_12m*: Number of credit inquiries in the last 12 months.
73. *default_ind*: A binary indicator (0 or 1) representing loan default status.

This dataset seems to contain various financial and personal information about borrowers and their loans, and the "default_ind" column is likely used to indicate whether a borrower has defaulted on their loan (1 for default, 0 for no default).


