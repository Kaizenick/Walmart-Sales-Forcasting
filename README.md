## Walmart Recruiting - Store Sales Forecasting:

- Walmart has provided historical sales data for 45 Walmart stores located in different regions. 
- Each store contains a number of departments, and we are tasked with predicting the department-wide sales for each store.
- In addition, Walmart runs several promotional markdown events throughout the year. 
- These markdowns precede prominent holidays, the four largest of which are the Super Bowl, Labor Day, Thanksgiving, and Christmas. 
- The weeks including these holidays are weighted five times higher in the evaluation than non-holiday weeks.
- Part of the challenge presented by this competition is modeling the effects of markdowns on these holiday weeks in the absence of complete/ideal historical data.


- The goal is to predict the Weekly Sales for the future dates that Walmart has given in test.csv file.
- This Kaggle competition is available at https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting

#### Data:
- The dataset essentially contains five scv files which are descibed as follows.

- train.csv:

    This is the historical training data, which covers to 2010-02-05 to 2012-11-01. Within this file we will find the following fields:

    - Store - the store number
    - Dept - the department number
    - Date - the week
    - Weekly_Sales - sales for the given department in the given store
    - IsHoliday - whether the week is a special holiday week
        
- stores.csv:
    
    This file contains anonymized information about the 45 stores, indicating the type and size of store.
    
- features.csv:

    This file contains additional data related to the store, department, and regional activity for the given dates. It contains the   following fields:

    - Store - the store number
    - Date - the week
    - Temperature - average temperature in the region
    - Fuel_Price - cost of fuel in the region
    - MarkDown1 to MarkDown5 - anonymized data related to promotional markdowns that Walmart is running. MarkDown data is only available after Nov 2011, and is not available for all stores all the time. Any missing value is marked with an NA.
    - CPI - the consumer price index
    - Unemployment - the unemployment rate
    - IsHoliday - whether the week is a special holiday week
    
 - test.csv:

    This file is identical to train.csv, except we have withheld the weekly sales. We must predict the sales for each triplet of store, department, and date in this file.

 - sampleSubmission.csv:

    We have been provided with dates where we can predict the salesfor each date mentioned in this csv file


