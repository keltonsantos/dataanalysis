# 🏀 NBA season 2021/2022 Case Study

<img src="images/projects/nba/home.JPG?raw=true">

### 📊 Project description

This project is part of the [Data Analytics Accelarator Bootcamp](https://www.datacareerjumpstart.com/) by [Avery Smith](https://www.linkedin.com/in/averyjsmith/). In this project, I'll pretend I am being interviewed by the NBA team the Utah Jazz for an Entry Data Analyst Role.

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

In this dataset, we have the following information 👇

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
* What position was the most efficient at shooting 3-pointers for every team?
* What are the total points scored by each team?
* What are the Top 10 Cape Verde Projects by amount disbursed?

## 📈 Analyses

To analyze our data, we will use **Tableau** for better data visualization.

### 1\. How different players did on total points, total assists, and total rebounds?

Let us create a bubble plot:


<img src="images/projects/nba/Bubble.PNG?raw=true">

As we can see, among all the players, Trae Young was the player with more points (2155) and assists (737) during the 2021-2022 NBA season. Nikola Jokić accumulated the most rebounds (1019). Chirs Paul was the second player with more assists (702) but got less than half of Young's points. 

Tyrese Haliburton was the player with more points (1181), assists (628), and rebounds (311) among the SG-PG (Shooting Guard and Point Guard) position players.
- - -

### 2\. What position was the most efficient at shooting 3-pointers for every team?

To answer this question, we will create a table representing the Teams on the y-axis and positions on the x-axis. As shown in the table below, the PF (Power Forward) position of the Sacrament Kings had the best 3-point shooting average (around 50%), followed by the SF (Small Forward) of the Los Angels Clippers (around 47%).

The Center position of the Utah Jazz had the worst successful 3-point average (around 0%).

<img src="images/projects/nba/table.png?raw=true">
- - -


### 3\. What are the total points scored by each team?

By plotting a **bar chart**, it's possible to see that Minnesota was the team with more points scored (9507), while Oklahoma scored less than all the teams (8506).



<img src="images/projects/nba/stacked_chart.png?raw=true">
- - -

### 4\. What players had more than 350 assists in every position?

 To accomplish this task, we will create a **tree map chrart** similar to the table in question 2.

<img src="images/projects/nba/tree_map.png?raw=true">

The solution is pretty straightforward, as we can see in the tree map above. The Player with more assists in every position are:

- PG (Point Guard) - James Harden
- SG (Shooting Guard) - Derrick White
- PF (Power Forward) - Giannis Antetokounmpo
- C (Center) - Nikola Jokić
- SF (Small Forward) - Khris Middleton

We can also notice that for Center position only Nikola Jokić made more than 350 assists, while for Small Forward only Khris Middleton reached 350 assists. No player in the positions of Guard and Forward made more than 350 assists.
- - -

## ✏️ Conclusion

- **Trae Young** was the player with more points (2155) and assists (737) during the 2021-2022 NBA season
- **Nikola Jokić** accumulated the most rebounds (1019)
- PF (Power Forward) position of the Sacrament Kings had the best 3-point shooting average (around 50%)
- Minnesota was the team with more points scored (9507)

- - -

Thank you for reading, if you have any feedback feel free to conect with on [LinkdIn](https://www.linkedin.com/in/kelton-garcia-santos-a75060b3/)