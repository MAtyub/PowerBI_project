# PowerBI_project

### In the Sample-superstore file I have created an interactive dashboard after cleaning and transforming the Sample-superstore dataset from Kaggle. It includes:

- Total sales and profit
- Sales by market
- Top 10 profit by country
- Top 10 sales by country

---

### In the Home_loan_eligibility project I have used few DAX and transformed data using Powerquery, and created an interactive dashboard to show custometr who are eligible for loan.

Data transformed in power query:
- Changed CustomerKey to int, and Name to text
- Replaced Homeowner and Gender values for better understanding
- Concatenated first & last name

Dax used:
- __To calculate age of customers__ : Age = DATEDIFF('Customer Table'[BirthDate],TODAY(),YEAR)

- __Used if statement : Loan Approval__ = IF('Customer Table'[Age] <= 60 && 'Customer Table'[HomeOwner] = "No" && 'Customer Table'[AnnualIncome] >= 40000, "Eligibile for Loan ", "Not Eligibile for Loan") 
