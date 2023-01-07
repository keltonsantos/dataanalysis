# IDA (World Bank) Statement of Credit and Grants - Cape Verde

### 📊 Project description

This project is part of the [Data Analytics Accelarator Bootcamp](https://www.datacareerjumpstart.com/) by [Avery Simth](https://www.linkedin.com/in/averyjsmith/).

#### About IDA (International Development Association)

The International Development Association (IDA) credits are public and publicly guaranteed debt extended by the World Bank Group. IDA provides development credits, grants and guarantees to its recipient member countries to help meet their development needs. Credits from IDA are at concessional rates. Data are in U.S. dollars calculated using historical rates. This dataset contains historical snapshots of the IDA Statement of Credits and Grants including the latest available snapshot. [Source: World Bank](https://finances.worldbank.org/Loans-and-Credits/IDA-Statement-Of-Credits-and-Grants-Historical-Dat/tdwh-3krx)

### 💾 The Data

The data for this project can be found on the website of [World Bank](https://finances.worldbank.org/Loans-and-Credits/IDA-Statement-Of-Credits-and-Grants-Historical-Dat/tdwh-3krx). We downloaded the CSV file from the website and imported it to SQL and Tableau for analysis.

In this dataset we have the following information 👇

* Nº Rows: 1.12 million
* Each row is a **Credit or Grant** at a specific time (month and year).
* Nº columns: 30

The main columns used in this project are:

* End of Period;
* Credit Number;
* Country;
* Credit Status;
* Project Name;
* **Disbursed Amount**;
* **Repaid to IDA**;
* **Due to IDA**

👉 Visit this [link](https://finances.worldbank.org/Loans-and-Credits/IDA-Statement-Of-Credits-and-Grants-Historical-Dat/tdwh-3krx) for more information about the dataset and data dictionary.

### 🕵️ The Task

We will analyze the loans and credit of IDA, and answer the following questions:

* What are the Top 10 debtors of IDA
* How much did Cape Verde disburse from 2012 to 2022?
* How much does Cape Verde owe to IDA?
* What are the Top 10 Cape Verde Projects by amount disbursed?

## 📈 Analyses

To analyze our data, we had to use **SQL** because the CSV file had more than 1 million rows, making it very difficult to use Excel.

### 2\. What are the Top 10 debtors of IDA?

To answer the first question, I executed the following **SQL** query, and used **Tableau** to plot the data:

``` sql
SELECT country, SUM ("Due to IDA") AS "Total_Due" 
FROM "IDA_Finance" 
WHERE "End of Period" = '12/31/2021 12:00:00 AM' 
GROUP BY "country"
ORDER BY "Total_Due" Desc
LIMIT 10;
```

<img src="images/projects/world_bank/top_10.png?raw=true">

As we can see India, Bangladesh,and Pakistan are the Top 3 debtors. The Top 10 countries are from the Asian and African Continent, as we can see below

<img src="images/projects/world_bank/map.png?raw=true">

### 2\. How much did Cape Verde disburse from 2012 to 2022?
By ploting the data, of disbursed amount, it's possible to see a trend in the stock of amout Cape Verde disbursed each year.

<img src="images/projects/world_bank/Stock_Disbursed.png?raw=true">

Taking a closer look to the individual amount disbursed for year, it's possible to see that from 2019 to 2021 the amout disbursed were significantly greater than in the previous years. This may be due to face the economic consequence of Covid-19.

<img src="images/projects/world_bank/Disbursment_year.png?raw=true">

### 3\. How much does Cape Verde owe to IDA?

First I filtered the data only for "Cape Verde" and "Cabo Verde" (they are the same country) using the following query:

``` sql
SELECT * 
FROM "IDA_Finance" 
WHERE "country" = ('Cabo Verde', 'Cape Verde');
```
As of November 2022, Cape Verde owed 458 Million USD to the World bank.

<img src="images/projects/world_bank/cv_debt.png?raw=true">

Cape Verde also repays to IDA every year, as we cans see in the chart below:

<img src="images/projects/world_bank/Stock_Repayment.png?raw=true">
Thank you for reading, if you have any feedback feel free to conect with on [LinkdIn](https://www.linkedin.com/in/kelton-garcia-santos-a75060b3/)