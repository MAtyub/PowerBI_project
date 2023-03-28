# PowerBI_project

### In the Sample-superstore file I have created an interactive dashboard after cleaning and transforming the Sample-superstore dataset from Kaggle. It includes:

- Total sales and profit
- Sales by market
- Top 10 profit by country
- Top 10 sales by country

![Screenshot 2023-03-28 145321](https://user-images.githubusercontent.com/116057738/228214214-fe73ecf2-8f66-419a-a6cf-9f302e212711.png)

---

### In the Home_loan_eligibility project I have used few DAX and transformed data using Powerquery, and created an interactive dashboard to show custometr who are eligible for loan.

Data transformed in power query:
- Changed CustomerKey to int, and Name to text
- Replaced Homeowner and Gender values for better understanding
- Concatenated first & last name

Dax used:
- __To calculate age of customers__ : Age = DATEDIFF('Customer Table'[BirthDate],TODAY(),YEAR)

- __Used if statement : Loan Approval__ = IF('Customer Table'[Age] <= 60 && 'Customer Table'[HomeOwner] = "No" && 'Customer Table'[AnnualIncome] >= 40000, "Eligibile for Loan ", "Not Eligibile for Loan") 


![Screenshot 2023-03-28 145149](https://user-images.githubusercontent.com/116057738/228214312-39caaac0-d67a-4176-9eab-49c1706f3f54.jpg)
