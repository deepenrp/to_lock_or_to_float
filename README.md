# to_lock_or_to_float


## Background

When going through the mortgage process there is that age old question on whether to Lock the loan or Float. With my experience talking to over 2000 Mortgage Loan Officers around the country, I have heard many strategies. 

Unfortunately, the most common answer among MLOs is to lock the loan as soon as possible. Some say that they lock after the loan has gone through underwriting and they know for sure that the loan is going to close. There are several services that help MLOs understand interest rate direction and manage the risks such as MBS Highway, Rate Alert, MBS Live, etc. While these services do a great job, their lock/float advice is not 100% accurate.

When purchasing a house there is a time period between going under contract and closing. This is the time period when most loans need a hedging strategy so that the best rate can be locked. This time frame can be a couple weeks to up to 3 months. There are a variety of factors that contribute to the decision making.

This repository attempts to assist in the decision making. 


## Data Source

In my opinion, we need enterprise level data from vendors such as Bloomberg, Thompson Reuters, or even proprietary data. to help create the machine learning models needed to assist our decision making. Nonetheless, this repo's attempt will utilize public data provided by the St. Louis Fed via their API. You will need your own API Key to run the queries needed for this project.

    * FRED API => https://fredaccount.stlouisfed.org/login/secure/


## Run

Step 1:- Enter your FRED API Key in the `{data_source}` jupyter notebook and save notebook.

Step 2:- Run the `{to_lock_or_to_float}` jupyter notebook. The 2nd cell will run the following jupyter notebooks:-

    * data_source.ipynb
    * inflation.ipynb
    * productivity.ipynb
    * jobs.ipynb
    * housing.ipynb
These notebooks create a proprietary index for their corresponding category. i.e. the inflation notebook creates an overall inflation index based on the datapoints fed into the analysis. There are also charts to help visualize the data.

Step 3:- More data wrangling and ML model tuning may be required.


Note:- The ML models in this repository will always be a work in progress due to the handicap of not utilizing vendor data and also experimenting on other ML models not included in the repository.

#### This repository is a work in progress and is in constant improvement.
