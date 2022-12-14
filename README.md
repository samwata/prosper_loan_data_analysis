# Prosper Loan Data Analysis
### By Samson Amwata

The dataset can be found [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv), with feature documentation available [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0)
You can also find the dataset and feature documentation under this repository

This dataset contains loan information of about 113,937 rows with 81 variables on each
loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.

I am looking forward to investigate the following questions
- What factors affect a loan’s outcome status?
- What affects the borrower’s APR or interest rate?
- Are there differences between loans depending on how large the original loan amount was?

## Data cleaning
Definition of data cleaning issues
- Remove duplicates rows
- Convert the date columns to date data type
- Rename ProsperRating (Alpha) column to ProsperRating
- Replace `NaT` dates to `Null`
- Add new columns Month and Year pulled from loanOriginateDate column
- We have `Not employed` and `Not displayed` in the list of ranges. We can replace this with `$0`
- Replace `True` and `False` values in `IsBorrowerHomeowner` to have `Yes` or `No`

## Summary of Findings
In this dataset, I am interested in borrowers features and features related to loan or those that affect loan performance.I am focused mainly on the original loan amount, borrower's rate, Prosper rating, loan term and borrower's stated monthly income.

I noticed that the Borrower Rate has positive correlation with the amount borrowed. The amount borrowed increased with higher ratings across all terms.
From the analysis I was able to find out that those borrowers with Full time job was getting lowest interest rate over time and those who are self employed and Not employed had high interest rate.
Also those employed and those with full time job got lowest interests compared with those who are not employed.


## Key Insights for Presentation
I focused on key features that will answer the questions for my investigation. I started by showing the amount of loan loaned out and to find out if the Borrower Rate, Prosper rating and APR rate has effect on the amount of loan borrowed.
Also I checked the correlation between different features 
