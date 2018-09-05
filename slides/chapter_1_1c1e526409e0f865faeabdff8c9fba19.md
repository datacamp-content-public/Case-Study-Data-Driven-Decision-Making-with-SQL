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
In the first case study, you built your first SQL query using Video Games Sales database. Your job was to accessing and interrogating data from the Sales table. Your aim was to analyse sales trend.

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

- Difference between WHERE and  HAVING when applying conditions in a SQL statement {{2}}


`@part2`
_What’s the total sales?_ {{3}}

``SELECT SUM(Global_Sales) AS TotalSales from Sales``{{4}}


`@part3`
_What’s the average sales?_ {{3}}

``SELECT AVG(Global_Sales) AS AvgSales from Sales`` {{5}}


`@script`
You practised your knowledge on SELECT statements and putting summarising functions. Furthermore we explored the use case of WHERE clause and HAVING. 

The HAVING clause was added to SQL because the WHERE keyword could not be used with aggregate functions.

The functions showed on the right were used to summarize numeric type of columns.

You were able to answer key questions like what’s the total sales to date.


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
For the second case study, we talked about love....or was it attraction? Using a data published on Kaggle which was compiled by Columbia Business School professors Ray Fisman and Sheena Iyengar for their paper Gender Differences in Mate Selection: Evidence From a Speed Dating Experiment. You learned how to 
 
SELECT DISTINCT is used to return only distinct (different) values.

So you discovered that there was a specific pattern demographic profile in this experiment?


---
## Speed Dating Experiment - Am I dateable?

```yaml
type: "TwoRowsWideBottom"
key: "7f5fb0a711"
```

`@part1`
_ How many data professionals are there in the speed dating experiment? _


`@part2`
SELECT


`@part3`
As a female Data Scientist aged 35, am I dateable?


`@script`



---
## Daily Happiness & Employee Turnover - JOIN tables

```yaml
type: "TwoRowsWideTop"
key: "91a89ca986"
```

`@part1`
What you have learned: {{1}}

- Difference types of JOINS {{2}}

- Combining result sets with UNION and UNION ALL {{3}}

- JOIN vs UNION {{4}}


`@part2`



`@part3`



`@script`
In the previous 2 case studies you had practice your skill on applying Select statement and aggregating data. In the 3rd case study you have learned about querying multiple tables thru the use of JOIN which is bread and butter of using SQL to accessing relational databases.

This third case study was about database that record daily happiness levels at work as used by myhappyforce.com app. You learned the concept of relational database which is bread and butter of SQL.

Let’s review our data scheme here


---
## Analysis of Refugee Crisis

```yaml
type: "TwoRowsWideTop"
key: "1fecb85d6d"
```

`@part1`
What you have learned: {{1}}


`@part2`



`@part3`



`@script`
The final case study was about Refugee Crisis Analysis - this chapter enabled you to choose practise different SQL syntax and functions learned from previous 3 chapters.


---
## Tips & Best Practise

```yaml
type: "FullCodeSlide"
key: "98312c63bc"
```

`@part1`
- Capitalise SQL keywords

  ``SELECT * FROM sales``

- Use Alias

- Avoid SELECT ALL statement if possible


`@script`
Although by not following these following tips may not break your code however its a good practise. Once you become the expert, which I think by the end of this course you will definitely are, you will get into the habit of writing SQL codes which is useful when working in a collaborative environment so that it is easy for your colleagues to pick up where you left off!

First, as previously mentioned, in some SQL environments it is not case sensitive, writing the code in lowercase or uppercase will not result in error however it makes the distinction between SQL keywords and non SQL keywords.


---
## Hope you enjoy the course!

```yaml
type: "FinalSlide"
key: "c4d5498aab"
```

`@script`


