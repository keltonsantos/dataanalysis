# IDA (World Bank) Statement of Credit and Grants - Cape Verde  

### 📊 Project description

 This project is part of the [Data Analytics Accelarator Bootcamp](https://www.datacareerjumpstart.com/) by [Avery Simth](https://www.linkedin.com/in/averyjsmith/).

#### About IDA (International Development Association)

The International Development Association (IDA) credits are public and publicly guaranteed debt extended by the World Bank Group. IDA provides development credits, grants and guarantees to its recipient member countries to help meet their development needs. Credits from IDA are at concessional rates. Data are in U.S. dollars calculated using historical rates. This dataset contains historical snapshots of the IDA Statement of Credits and Grants including the latest available snapshot. [Source: World Bank](https://finances.worldbank.org/Loans-and-Credits/IDA-Statement-Of-Credits-and-Grants-Historical-Dat/tdwh-3krx)

### 💾 The Data
The data for this project can be found on the website of [World Bank](https://finances.worldbank.org/Loans-and-Credits/IDA-Statement-Of-Credits-and-Grants-Historical-Dat/tdwh-3krx).  We downloaded the CSV file from the website and imported it to SQL and Tableau for analysis.

In this dataset we have the following information 👇

- Nº Rows: 1.12 million
- Each row is a **Credit or Grant** at a specific time (month and year).
- Nº columns: 30

The main columns used in this project are:
- End of Period;
- Credit Number;
- Country;
- Credit Status;
- Project Name;
- **Disbursed Amount**;
- **Repaid to IDA**;
- **Due to IDA**

👉 Visit this [link](https://finances.worldbank.org/Loans-and-Credits/IDA-Statement-Of-Credits-and-Grants-Historical-Dat/tdwh-3krx) for more information about the dataset and data dictionary.

### 🕵️ The Task 

We will analyze the loans and credit of IDA, and answer the following questions:

- Which country has the most debt to IDA?
- What are the Top 10 debtors of IDA
- How much did Cape Verde disburse from 2012 to 2022?
- How much does Cape Verde owe to IDA?
- What are the Top 10 Cape Verde Projects by amount disbursed?

## 📈 Analyses

We connected our csv file to tableau public to analyze and visualize the data and address the questions to present to the board of the school.

<img src="images/projects/Mass_tableau/data.PNG?raw=true">

### 1\. What schools are struggling he most?

To answer this question, we built a **bar chart** to find out the bottom 10 schools with the lowest graduation rate. We created a bar chart where the graduation percentages were displayed for each school. In the **bar chart** below, we can see the schools that are struggling the most.

<img src="images/projects/Mass_tableau/bar_chart.PNG?raw=true">

### 2\. What are the top math schools in the state?

The school board wanted to find out what the top math school was in the state. They believed that 4th grade math is key to a student's feature and would like to focus on improving the state's MCAS 4thGrade Math passing grade. They wanted to know which districts were above the desired threshold of 50% and would like to collect the names of these districts to invite some of these teachers to train the rest of the state on how they improve math scores.

By plotting the percentage of "MCAS 4th Grade Math", and setting a threshold of 50% we got the top math schools.

* Community Day Charter Public School — R. Kingman Webster (District)
* Community Day Charter Public School — Prospect (District)
* Community Day Charter Public School — Gateway (District)
* Orleans

<img src="images/projects/Mass_tableau/math.PNG?raw=true">

### 3\. How does class size affect college admission?

The school board is wondering how college attendance would be increased. They're considering investing in building more schools in the aim of lowering the average class size to hopefully increase the % attending college.

Plotting the scatter plot of "Average Class Size" and "% Attending College", we found an R-squared of 0.19, which means that keeping all other variables constants, "Class Size" only explains 19% of variability of "College Attendance". An R-squared of 19% is too small to conclude that there is casual relationship between "Average Class Size" and "% Attending College".

<img src="images/projects/Mass_tableau/scatter.PNG?raw=true">

## 📓 Conclusion

The State of Massachusetts has 1,861 schools and 953,859 students;
Four schools passed the 4th grade math threshold set by the board school;
The average class size is 18 students per class;
There is no strong correlation between class size and class attendance.

<img src="images/projects/Mass_tableau/dashboard.PNG?raw=true">

Thank you for reading, if you have any feedback feel free to conect with on [LinkdIn](https://www.linkedin.com/in/kelton-garcia-santos-a75060b3/)