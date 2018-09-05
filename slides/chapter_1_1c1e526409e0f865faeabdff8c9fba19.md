---
title: Insert title here
key: 1c1e526409e0f865faeabdff8c9fba19

---
## Wrapping up

```yaml
type: "TitleSlide"
key: "e1ba3c4dcb"
```

`@lower_third`

name: Nujcharee Haswell (Ped)
title: Data and Intelligence Specialist / Data Scientist


`@script`
Congratulations! You have completed the final case study in this course on data driven decision making with SQL.

Now let's summarise what you have learned in this course.


---
## Video Game Sales - Basic SQL query

```yaml
type: "TwoRowsWideBottom"
key: "d7b537ab21"
```

`@part1`
What you have learned: {{1}}

- Basic understanding of relational database components such as tables, columns, rows and keys {{2}}
- Basic SQL query using 3 keywords SELECT...FROM...WHERE {{3}}


`@part2`
_What video games sold in year 2006 worldwide?_ {{4}}


`@part3`
Sample SQL Queries {{5}}

``SELECT * FROM Sales WHERE Year = 2006`` {{6}}

 ``SELECT Year, Publisher, Revenue FROM Sales WHERE Year = 2006`` {{7}}


`@script`
In the first case study, you built your first SQL query using Video Game Sales database. Your job was to accessing and interrogating data from the Sales table. Your aim was to analyse sales trend.

What you have learned:

Basic understanding of relational database components such as tables, columns, rows and keys

Then, you learned to apply SELECT...FROM...WHERE statement which is a basis of a simple SQL query to initially explore the data in the table.

You were able to answer a question  "What video games sold in year 2006 worldwide?" by using these sample queries here.


---
## Video Game Sales - Summarising data

```yaml
type: "TwoRowsWideBottom"
key: "72edb8fdcd"
```

`@part1`
What you have learned: {{1}}

- Summarising data using aggregated functions such as SUM and AVG {{2}}

- Difference between WHERE clause and HAVING clause when applying conditions in a SQL statement {{2}}


`@part2`
_What’s the total sales?_ {{3}}

``SELECT SUM(Global_Sales) AS TotalSales from Sales``{{4}}


`@part3`
_What’s the average sales?_ {{3}}

``SELECT AVG(Global_Sales) AS AvgSales from Sales`` {{5}}


`@script`
Furthermore you explored the use case of summarising data using aggregated functions such as SUM and AVG

Then you learned about difference between WHERE clause and HAVING clause when applying conditions in a SQL statement {{2}}
The HAVING clause was added to SQL because the WHERE keyword could not be used with aggregated functions.

You were able to answer key questions like 

What’s the total sales to date.
What’s the average sales?


---
## Speed Dating Experiment - beyond SELECT statement

```yaml
type: "TwoRowsWideTop"
key: "f73afe007d"
```

`@part1`
What you have learned: {{1}}

- Use SELECT DISTINCT statement {{2}}

- Apply ORDER BY to sort result set {{3}}

- Include / exclude missing values by applying IS NULL {{4}}

- Calculate columns using CASE WHEN {{5}}


`@part2`
Code Samples {{2}}

``SELECT DISTINCT career FROM SpDates`` {{2}}

``SELECT career, age, score FROM SpDates ORDER BY age`` {{3}}

``SELECT * FROM SpDates WHERE race IS NULL`` {{4}}


``SELECT gender, CASE WHEN score > 10 THEN 'Good' ELSE 'Not a good match' END AS result FROM SpDates`` {{6}}


`@part3`



`@script`
For the second case study, we talked Evidence from a Speed Dating Experiment database published on Kaggle which was compiled by Columbia Business School.
 
You applied the use of SELECT DISTINCT to return only distinct (different) values.

Later, you learned to apply keyword ORDER BY to sort result set - as per the sample here.

In general, if dataset contains a lot of incomplete records, it will not be useful therefore IS NULL can be used to quantify number of rows with missing data.

Finally, you applied calculated columns using CASE WHEN to evaluate conditions, very similar to IF...ELSE


---
## Must be love at first sight?

```yaml
type: "TwoRowsWideBottom"
key: "7f5fb0a711"
```

`@part1`
Exploring ``SpDates`` table in the database to answer following questions; {{1}}

- How many scientist profession are there in the speed dating experiment? {{2}}

``SELECT id, age, gender FROM SpDates WHERE career = 'Scientist'``  {{3}}

- Sort the result set by age of participants {{4}}

``SELECT id, age, gender FROM SpDates WHERE career = 'Scientist' order by age`` {{5}}
 
- How many would like to see their date again? {{6}}

``SELECT id, age, gender FROM SpDates WHERE career = 'Scientist' AND matched = 1`` {{7}}


`@part2`



`@part3`



`@script`
You were able to answer following questions;

How many scientist profession are there in the speed dating experiment?

Next, you improved the statement by adding ORDER BY to sort the result set by age

Finally, you discover the number of participants who would like to see their date again using this query.


---
## Daily Happiness & Employee Turnover - JOIN tables

```yaml
type: "TwoRowsWideTop"
key: "91a89ca986"
```

`@part1`
What you have learned: 

- A JOIN clause is used to combine rows from two or more tables, based on a related column between them

- Use INNER JOIN when you need only rows that match on both side

![](https://github.com/nujcharee/courses/blob/master/Screen%20Shot%202018-09-05%20at%2018.21.50.png?raw=true) {{3}}


`@part2`
**Sample code ** 

``SELECT dept.staffid, dept.office, workers.gender, workers.age 
FROM workers INNER JOIN dept on workers.staffid 
= dept.staffid``


`@part3`



`@script`
The third case study we worked on a database about happiness levels at work as used by myhappyforce.com app. Joining multiple tables thru the use of JOIN is the bread and butter of using SQL with relational databases. This topic warrants a whole course in itself, there is a Joining data with PostgresSQL on DataCamp if you wish to deep dive into the subject.

So in this chapter you have learned

- Concept of JOIN clause, it is used to combine rows from two or more tables, based on a related column between them. There are many types of joins

First,

Use INNER JOIN when you need only rows that match on both side

You have examined the sample code right here which would give you the result set as per the screenshot here. Noticed that the INNER JOIN returned two rows that shared the common key "staffid" as highlighted in yellow.


---
## Daily Happiness & Employee Turnover - LEFT JOIN

```yaml
type: "TwoColumns"
key: "616164b2a4"
```

`@part1`
What you have learned: 

- Use LEFT JOIN to get optional values from another table(s)

![](https://github.com/nujcharee/courses/blob/master/Screen%20Shot%202018-09-05%20at%2018.27.42.png?raw=true) {{3}}


`@part2`
**Sample code ** 

For LEFT JOIN

``SELECT dept.staffid, dept.office, workers.gender, workers.age 
FROM workers INNER JOIN dept on workers.staffid 
= dept.staffid``


`@script`
Next, you have learned the use case of LEFT JOIN to get optional values from another table(s) by using the sample code here, it gave you the result set as per the screenshot here. Noticed that the LEFT JOIN returned four rows from the left table and showed the information from the right table where common key were shared - which was "staffid" as highlighted in yellow.


---
## Daily Happiness & Employee Turnover - RIGHT JOIN

```yaml
type: "TwoColumns"
key: "a02b6e3813"
```

`@part1`
- Same with RIGHT JOIN

![](https://github.com/nujcharee/courses/blob/master/Screen%20Shot%202018-09-05%20at%2018.24.59.png?raw=true) {{3}}


`@part2`
**Sample code ** 

``SELECT dept.staffid, dept.office, workers.gender, workers.age 
FROM workers INNER JOIN dept on workers.staffid 
= dept.staffid``


`@script`
The same goes with RIGHT JOIN, it gave the optional values from another table(s) by using the sample code here, it gave you the result set as per the screenshot here. Noticed that the RIGHT JOIN returned four rows from the right table and showed the information from the left table where common key were shared - which was "staffid" as highlighted in yellow.


---
## How happy are you at work today?

```yaml
type: "TwoRows"
key: "f9562f5ae0"
```

`@part1`
Explored the database to answer following questions; {{1}}

- When is the happiest day to be at work? {{2}}

``SELECT date.dayofweek, SUM(votes.likes) AS allvotes FROM dates INNER JOIN votes WHERE votes.date = dates.date GROUP BY date.dayofweek``  {{3}}
 
- How many negative votes before they get fired? {{4}}

``SELECT COUNT(votes.date) AS cnt, churn.employee from votes INNER JOIN churn on votes.employee = churn.employee WHERE churn.stillExisted = FALSE GROUP BY churn.employee HAVING votes.vote >0`` {{5}}


`@part2`



`@script`
You discovered that the database could answer the following questions

When is the happiest day to be at work?

How many negative votes before they get fired?


---
## Analysis of Refugee Crisis - Applying advanced SQL

```yaml
type: "TwoRows"
key: "aec538773d"
```

`@part1`
The final case study was about analysis of refugee crisis

In this chapter:

- Practise on skills learned from previous 3 chapters

- Capitalise SQL keywords

  ``SELECT * FROM sales``

- Use Alias for table name and / or column names

- Avoid SELECT ALL statement if possible


`@part2`



`@script`
The final case study was about Refugee Crisis Analysis - this chapter you practised different SQL syntax and functions learned from previous 3 chapters with tips and techniques here.

Awesome! You are on your way to be the expert in writing SQL and keep practising!


---
## Hope you enjoy the course!

```yaml
type: "FinalSlide"
key: "c4d5498aab"
```

`@script`


