# ProsperLoan Data analysis and exploration
## by Maximilien Kpizingui


## Dataset

ProsperLoan dataset contains 113,937 observations and 81 features from Prosper: a peer-to-peer lending platform. The dataset can be found [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv) and a detailed description of all the features can be found [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit).

## Summary of Findings

In wrangling the dataframe, I found that there was 1364086 missing and some features which were not of  interest in our analysis. Those irrelevant features and missing value were dropped and we created a loan masrter dataframe containing the clean data. In univariante exploration, we found unusual distribution in StatedMonthlyIncome it was highly skewed to the right. We use log scale to transform the data for better visualisation. Furtermore, in bivariante exploration, we notice that EmploymentStatus has a relationship with ProsperRating where the unemployed are mostly given a High Risk rating and the number of Defaulted loans for Self-employed people are larger than those for Not Employed. Moreover, We saw strong correlations between features like BorrowerAPR, BorrowerRate and EstimatedEffectiveYield; between MonthlyLoanPayment and LoanOriginalAmount; between ProsperScore and ProsperRating (Alpha). finally, in multivariante exploration,we found positive correlation between LenderYield and BorrowerAPR. We also noticed that most of loan applicants with lower BorrowerAPR and LenderYield have higher ProsperScore. We figured out from the exploration that Full-Time and part-time tend to have higher ProsperScore and lower BorrowerAPR,Not-Employed and Self-Employed tend to have lower ProsperScore and higher BorrowerAPR and Retired people have higher ProsperScore and lower BorrowerAPR


## Key Insights for Presentation

In my slide deck, I am going to focus on the correlation of the Original Loan Amount, ProsperRating on the BorrowerAPR. Besides, I explore how the BorrowerAPR may affect the loan status.
