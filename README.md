# Lending Club Case Study
> Performing EDA on a Loan Dataset from a Bank and provide inferences on the parameters which influences the probability of default and provide any other meaningful references

## NOTE : Please change the location from where you are reading the loan file in the Jupyter notebook, before running Jupyter Notebook
loan_df = pd.read_csv(r"C:\Users\Niraj\Downloads\loan\loan.csv", dtype=object) to appropriate location


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Provide general information about your project here.
- What is the background of your project?
  You work for a consumer finance company which specializes in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:
If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company
The data given below contains information about past loan applicants and whether they ‘defaulted’ or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.
In this case study, you will use EDA to understand how consumer attributes and loan attributes influence the tendency of default.
When a person applies for a loan, there are two types of decisions that could be taken by the company:
Loan accepted: If the company approves the loan, there are 3 possible scenarios described below:
Fully paid: Applicant has fully paid the loan (the principal and the interest rate)
Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.
Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan
Loan rejected: The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)

- What is the business probem that your project is trying to solve?
  This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface.
Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'.
If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.
In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default. The company can utilize this knowledge for its portfolio and risk assessment.
To develop your understanding of the domain, you are advised to independently research a little about risk analytics (understanding the types of variables and their significance should be enough).

- What is the dataset that is being used?
  Loan Dataset given by Upgrad

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- DEFAULT LOAN PATTERNS – INDICATORS OF DEFAULT
  - Very High Contributors
    - Lower Grades - Grades in E, F, G
    - Earlier Bankruptcies - Previously Recorded Bankruptcies
    - Higher Interest Rate – Interest Rate >10
    - High Debt to Income Ratio - DTI > 15
  - High Contributors
    - Lower Annual Income - <60K
    - Higher Loan Amount - >15K
    - Non Urban Borrowers – Not in California, NewYork, Florida, Texas, New-Jersey
    - Small Business Loans
- OTHER INFERENCES
  - Surprising Inferences - Immediate Actions
    - Currently Bank gives Higher Loan Amount on an Average to Grades in G, F, E in the same order than for A, B and C, which needs to be evaluated
    - Verified Loans and Source Verified Loans have higher percentage of Charged Off Loans, process of verification needs to be relooked
  - What is good and should be continued
    - Interest Rate is Inversely proportional to the Grade
    - As the Loan Amount increases Interest Rate also increases
    - Small Business have Higher Interest Rates
    - Interest Rate increases with Term



## Technologies Used
- Jupyter Notebook - Version: 7.2.2
- library - Numpy - 1.26.4, Pandas - 2.2.2, Matplotlib - 3.9.2, Seaborn- 0.13.2, Plotly - 5.24.1

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
This project is for Lending club case study assignment.
Team Members :Nishu Kumari,  Niraj Ram S, 


## Contact
Created by [@nishu-qatech] - feel free to contact me!
