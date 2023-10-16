# Homework 1
## SELECT queries 101

```
SELECT * FROM TABLE;
```
Another one is to display specific column is following:

```
SELECT COLUMN1, COLUMN2 FROM TABLE;
```

### Task 1
Displaying emails of payers, recipients and sum, and the SQL statement is shown below.
```
SELECT payer_email, recipient_email, sum FROM BILLING;
```

### Task 2
This is a SQL statement, which displays all sums larger than 900.
```
SELECT * FROM BILLING WHERE SUM > 900;
```
Second one is a SQL statement, which displays all sums larger than 900 OR less than 200.
```
SELECT * FROM BILLING WHERE SUM > 900 OR SUM < 200;
```
Third is a SQL statement, which displays all currencies equal to indian rupies and US dollars.
```
SELECT * FROM BILLING WHERE currency = "INR" OR currency = "USD";
```
Last, is a SQL statement within range of two values 750 and 800.
```
SELECT * FROM BILLING WHERE sum BETWEEN 750 AND 800;
```

### Task 3
Below, there is a SQL statement ordering by billing date in descending way.
```
SELECT * FROM BILLING ORDER BY billing_date DESC;
```
Also, there is a SQL statement ordering by billing date in asscending way.
```
SELECT * FROM BILLING ORDER BY billing_date ASC;
```
Last, we derived is a SQL statement ordering USD transcations by sum in descending way.
```
SELECT * FROM BILLING WHERE currency = "USD" ORDER BY sum DESC;
```