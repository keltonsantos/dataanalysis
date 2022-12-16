# Massachusetts School Project with Tableau :school:

### Project description

For this project we used *TABLEAU* to analyze education data of the state of Massachusetts, build a report to show the school board the state of the school system and answer the following questions:

* What schools are struggling the most?
* What are the top math schools in the state?
* How does class size affect college admission?

To address these questions, we used [Tableau Public](https://public.tableau.com/app/discover) to analyze and visualize the data. During the project we used the following tableau features:

-  Connecting to Data
-  Creating a bar chart
-  Adding color
-  Creating a scatter plot
-  Adding size
-  Adding label
-  Adding tooltip
-  Creating pie chart
-  Creating line chart
-  BAN / KPI / Metric
-  Reference Line

## Analyses

We upload our csv file to tableau public to analyze and visualize the data and address the questions to present to the board of the school.

<img src="images/projects/Mass_tableau/data.PNG?raw=true">

### 1\. What schools are struggling he most?

To answer this question, we built a bar chart to find out the bottom 10 schools with the lowest graduation rate. We created a bar chart where the graduation percentages are displayed for each school. In the **bar chart** below, we can see the schools that are struggling the most.

<img src="images/projects/Mass_tableau/bar_chart.PNG?raw=true">

### 2\. What are the top math schools in the state?

The school board wanted to find out what the top math school was in the state. They believed that 4th grade math is key to a student's feature and would like to focus on improving the state's MCAS 4thGrade Math passing grade. They wanted to know which districts were above the desired threshold of 50% and would like to collect the names of these districts to invite some of these teachers to train the rest of the state on how they improve math scores.

By plotting the percentage of "MCAS 4th Grade Math", and setting a threshold of 50% we got the top math schools.

- Community Day Charter Public School — R. Kingman Webster (District)
- Community Day Charter Public School — Prospect (District)
- Community Day Charter Public School — Gateway (District)
- Orleans

<img src="images/projects/Mass_tableau/math.PNG?raw=true">

### 3\. How does class size affect college admission?

 The school board is wondering how college attendance would be increased. They're considering investing in building more schools in the aim of lowering the average class size to hopefully increase the % attending college.

Plotting the scatter plot of "Average Class Size" and "% Attending College", we found an R-squared of 0.19, which means that keeping all other variables constants, "Class Size" only explains 19% of variability of "College Attendance". An R-squared of 19% is too small to conclude that there is casual relationship between "Average Class Size" and "% Attending College".

<img src="images/projects/Mass_tableau/scatter.PNG?raw=true">

## Conclusion

The State of Massachusetts has 1,861 schools and 953,859 students;
Four schools passed the 4th grade math threshold set by the board school;
The average class size is 18 students;
There is no strong correlation between class size and class attendance.

<img src="images/projects/Mass_tableau/dashboard.PNG?raw=true">


For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).