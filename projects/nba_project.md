# NBA season 2021/2022 Case  Study

<img src="images/projects/nba/home.JPG?raw=true">

### 📊 Project description

This project is part of the [Data Analytics Accelarator Bootcamp](https://www.datacareerjumpstart.com/) by [Avery Simth](https://www.linkedin.com/in/averyjsmith/). In this project, I'll pretend I am being interviewed by the NBA team the Utah Jazz for an Entry Data Analyst Role.

**Topics covered**:

✅ Multiple Data Sources
✅ Scatter plot
✅ Bubble plot
✅ Area Chart
✅ Heatmap 
✅ Drill down
✅Tableau Stories
✅Detail
✅Tooltip


### 💾 The Data

The data for this project can be found [HERE](https://www.basketball-reference.com/leagues/NBA_2022_totals.html). We downloaded the CSV file from the website and imported it to **Tableau** for analysis.

In this dataset we have the following information 👇

* Nº Rows: 605
* Each row is the **statistic of a unique player** in 2021/2022 NBA season.
* Nº columns: 30

The main columns used in this project are:

* Player;
* POS - Position;
* Age;
* Tm - Team;
* G- Games;
* FG - Field Goals;
* 3P - 3 Points Field Goal;
* FT - Free Throws
* AST - Assist
* (...)

👉 Visit this [link](https://www.basketball-reference.com/leagues/NBA_2022_totals.html) for more information about the glossary of dataset.

### 🕵️ The Task

We will analyze the data, and answer the following questions:

* How different players did on total points, total assists, and total rebounds?
* How much did Cape Verde disburse from 2012 to 2022?
* How much does Cape Verde owe to IDA?
* What are the Top 10 Cape Verde Projects by amount disbursed?

## 📈 Analyses

To analyze our data, we will use **Tableau** for better data visualization.

### 1\. How different players did on total points, total assists, and total rebounds?

Let us create a bubble plot:


<img src="images/projects/nba/home.JPG?raw=true">

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

Cape Verde also repays to IDA every year, as we can see in the chart below:

<img src="images/projects/world_bank/Stock_Repayment.png?raw=true">

### 4\. What are the Top 10 Cape Verde Projects by amount disbursed?

After plotting a bubble chart, we can see that the top projects, by amount disbursed are:

- Cabo Verde - Transport Sector Reform
- Cabo Verde DPO
- Cabo Verde DPF FY22
- (...)

<img src="images/projects/world_bank/Projects.png?raw=true">

## ✏️ Conclusion

- The Top Five countries with the most amount due to IDA are, **India**, **Bangladesh**, **Pakistan**, **Nigeria** and **Vietnam**
- As of Nov 2022, Cape Verde owed about 458 Million USD to IDA.
- The stock of repayment Cape Verde made to IDA was 96.6 Million USD as of Nov2022.



Thank you for reading, if you have any feedback feel free to conect with on [LinkdIn](https://www.linkedin.com/in/kelton-garcia-santos-a75060b3/)