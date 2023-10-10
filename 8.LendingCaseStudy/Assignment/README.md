# Lending Club Case Study
> This project was done as part of assignment of the course Master of Science in Machine Learning & AI from Liverpool John Moores University, through Upgrad.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)



## General Information

You work for a  **consumer finance company ** which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant's profile. Two  **types of risks**  are associated with the bank's decision:

- If the applicant is ** likely to repay the loan** , then not approving the loan results in a  **loss of business**  to the company
- If the applicant is  **not likely to repay the loan,**  i.e. he/she is likely to default, then approving the loan may lead to a  **financial loss**  for the company

The data given below contains information about past loan applicants and whether they 'defaulted' or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.

In this case study, you will use EDA to understand how  **consumer attributes**  and  **loan attributes**  influence the tendency of default.

When a person applies for a loan, ** ** there are ** two types of decisions**  that could be taken by the company:

1. **Loan accepted:**  If the company approves the loan, there are 3 possible scenarios described below:
  - **Fully paid** : Applicant has fully paid the loan (the principal and the interest rate)
  - **Current** : Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.
  - **Charged-off** : Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has  **defaulted ** on the loan
2. **Loan rejected** : The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)

### Business Objective

This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface.

Like most other lending companies, lending loans to 'risky' applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who  **default**  cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'.

If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.

In other words, the company wants to understand the **driving factors (or driver variables) **behind loan default, i.e. the variables which are strong indicators of default.  The company can utilise this knowledge for its portfolio and risk assessment.

### Data Set

The dataset, loan.csv can be found in the github repo. It contains the complete loan data Liverpool John Moores University, through Upgradfor all loans issued through the time period 2007 t0 2011.

The data dictionary,Data\_Dictionary.xlsx which describes the meaning of these variables is in this github repo.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Most of the Loan amounts are in range of 5000 - 10000
- Most of the  Interest Rates on loans are in range of 12% - 15%
- When Anual income is low  then dti is high and vice versa
- Annual income increases by employement length
- Loan amount also increases with increase in annual_inc and also the installment increases with annual inc
- 85% of the Loan is fully paid and 15% of the loan is charged off
- As per purpose of the loan most of the loans taken for debt consolidation(47%) and Credit card bill payment Other category is also one of the main area where loans were taken.
- It is observed that Mortgage and Rent home owenrs contribute towards the defaulter
- Most of the loans were taken for the purpose of debt consolidation & paying credit card bill. Number of chraged off count also high too for these loans.
- Most of the people living in rented home or mortgazed their home are major defaulters .Applicant numbers are high from these categories so charged off is high too.
- Those who had taken loan to repay in 36 months had more % of number of applicants getting charged off as compared to applicants who had taken loan for 60 months.
- Charged off is seen more when the interest rates are between 13-17% and 9-13%
- Charged off is more for people with work experience 10 years or with experice of 1 year
- Charged off is seen more when the open acc groups (The number of open credit lines in the borrower's credit file) is between 2-10 
- Charged off is seen more when the total_acc (The total number of credit lines currently in the borrower's credit file) is between 2-20 and then 20-37 
- Charged off is seen more when the annual inc is between 3k to 58k. More defaulters are seen in the annula income between 3K - 31K
- More defaulters are seen when the application is not verified and also for verified application
- More defaulters are seen when the inquiries in last 6 months is between 0-3
- More defaulters are seen when the  Number of derogatory public records is 0
- Charged off is seen more in dec 2011
- More defaulters are seen for 145-274 installment group
- More defaulters are seen for funded_amt_inv ammount between 5k-10k
- More defaulters are seen for 5k-10k loam amount
- More defaulters are seen for 12-18 dti group, however more defaulters are seen from 6-24 dti with 12-18 dti is the highest.
- Grade "F" and "G" have very high chances of charged off.Chances of charged of is increasing with grade moving from "A" towards "G"
- Charge off is seen more in home_improvement and house and these people had low income in that purpose than the people who fully paid. 
- Applicants with higher salary mostly applied loans for "home_improvment", "house","renewable_energy","credit_card" and "small_businesses"


## Technologies Used
- numpy - version 1.23.5
- pandas - version 1.5.3
- matplotlib - version 3.8.0
- seaborn - version 0.12.2
- warnings - version 3.10.0


## Acknowledgements

- This project was done as part of assignment of the course Master of Science in Machine Learning & AI from Liverpool John Moores University, through Upgrad


## Contact

- Anshuman Biswal
  - Github username [@anshumanbiswal26121981]

- Abhijit Kumar Manna
  - Github username [@]

**feel free to contact us!**


## License

MIT License

Copyright (c) [year] [fullname]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
