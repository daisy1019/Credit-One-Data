# Credit-One-Data

**Introduction**

Thsi report aims to find solutions to decrease customer default paymet rate and improve customers' payment performance. Please see the following findsing and suggestion:

**Problem 1 - predict who is likely to default payment**

**_odel used for prediction - DecisionTreeClassifier_**

We’ve run through both Regression and Classification models to determine that Classification method would produce a higher accuracy score, as classification method is suitable for large dataset, while regression method works better on a smaller dataset.

Here is our findings:
Customers who tend to **default payment**
1). Customers who are under age 57, married or with ‘other’ marital status, with limit balance given ≤ 450.000 usually pay their bills on time.
2). Female customers who are under age 53 with ≤ 355.000 limit balance tend to default payment. 

Customer who tend **not to default payment**
1). Customers who are under age 25, married or with marital status ‘others’ with a given credit limit ≤ 450.000 tend not to default payment
2). Married customers or with marital status ‘others’ who are under 45, with the credit limit ≤ 150.000 usually pay their bills on time.

**Problem 2 - need to predict how much credit limit customers should be assigned**

**_Model used for prediction - DecisionTreeClassifier _** - same as what we used for problem 1.


Here is our predictions:
 ≤ 100.000
1). Female customers who are under 25 with pay amount 6 ≤ 2002.5 should be assigned no more than this credit balance
2). Customers who have pay amount 6 ≤ 2002, pay amount 2 ≤ 7000, pay amount ≤ 2518 should be given 100.000 credit limit and under.

≤ 140.000
Customers who are under 25 with a graduate school education with pay amount 6 ≤ 2002 would be assigned this credit limit.

≤ 200.000
Customers with pay amount 1 ≤ 10002, pay amount 2 ≤ 7000, pay amount 6 ≤ 2002 should be given 200.000 credit limit and under. 

**More factors that affect who default vs. not default:

Default Payment vs.Education**

![image](https://user-images.githubusercontent.com/80385435/188296365-3c75f1b1-cd1f-4e16-bc4e-f582fa752f58.png)

Clients with university degree tend to default less, clients with high school level
education tend to default more.

**Default Payment vs. Marriage with Sex**

![image](https://user-images.githubusercontent.com/80385435/188296384-b6c73cb7-3fa2-464e-b3e6-c34c581f2b90.png)

Not Default
- Married females tend not to default more than married males
- Single males tend not to default more than females

Default
- Married females tend to default more than males
Single males tend to default more than females

We can decrease the credit limit for customer who tend to default payment and increase the credit limit for customer who pay their bills on time or reward in some other ways. 

**Recommendations**

The below heat map plot shows that there is very little to none correlation between different variables, Credit One might need to consider other factors to reduce default payment rate and to increase overall revenue for the company.

![image](https://user-images.githubusercontent.com/80385435/188296409-d767fb92-69f7-45ea-9ab3-2061338fbbf4.png)


**Factors need to consider:**

- Income ( do customers make enough money to cover their bills?)

- Debt ( how much do customer own, how much credit are they using?)

- Current accounts ( how many accounts do they have open for what type of loans?)

- Account history( how long they have for current accounts, and how many more new accounts they’ve been opened recently?)


**Reward customers with good payment history:**

- Higher credit limit can be offered

- Vouchers can be rewarded to good customers
