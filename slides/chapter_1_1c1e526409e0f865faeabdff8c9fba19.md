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

- Basic understanding of relational database components such as tables, column, rows and keys {{2}}
- Basic SQL query using 3 keywords SELECT...FROM...WHERE {{3}}


`@part2`
What video games sold in year 2006 worldwide? {{4}}


`@part3`
Sample {{5}}

``SELECT * FROM Sales WHERE Year = 2006`` {{6}}

 ``SELECT Year, Publisher, Revenue FROM Sales WHERE Year = 2006`` {{7}}


`@script`
The first case study was to interrogate the Sales table in the Video Games Sales database. Your job was to analyse sales trend as well as to summarise sales by regions group by publisher and year.

You learned: 

Basic understanding of relational database components such as tables, column, rows and keys

Then, you learned to apply SELECT...FROM...WHERE statement to initially explore the data.


---
## Video Game Sales - Summarising data

```yaml
type: "TwoRowsWideBottom"
key: "72edb8fdcd"
```

`@part1`
- Summarising data using SUM, AVERAGE, MIN and MAX {{1}}

- Difference between WHERE and  HAVING when applying conditions in a SQL statement {{2}}


`@part2`
> What’s the total sales? {{3}}


`@part3`
- ``SUM`` Total sales by product category {{4}}
- ``AVG`` Average sales by product category {{5}}
- ``MIN`` & ``MAX`` – Discover products with lowest and highest price per unit {{6}}


`@script`
Now that you learned about building a basic SQL SELECT statement, you found a way to improve this query by applying aggregated functions

The functions showed on the right were used to summarize numeric type of columns.

You were able to answer key questions like what’s the total sales to date.


---
## Speed Dating Experiment

```yaml
type: "TwoRowsWideTop"
key: "f73afe007d"
```

`@part1`
You learned how to:

- Use SELECT DISTINCT statement
- Apply ORDER BY to sort result set 

- Include / exclude missing values by applying IS NULL 

- Filter rows using AND, OR, and NOT operators 

- Apply Pattern matching with LIKE, wildcard (%) and IN operators

- Calculate columns using CASE WHEN


`@part2`
Code Samples

``SELECT DISTINCT career FROM SpDates``

``SELECT * FROM SpDates ORDER BY age``

``SELECT * FROM SpDates WHERE race IS NULL``

``SELECT * FROM SpDates WHERE career LIKE '%Data%' AND age in (30,31,32,33,34,35)``

``SELECT gender, CASE WHEN score > 10 THEN 'Good' ELSE 'Not a good match' END AS result
 FROM SpDates``


`@part3`



`@script`
For the second case study, we talked about love....or was it attraction? Using a data published on Kaggle which was compiled by Columbia Business School professors Ray Fisman and Sheena Iyengar for their paper Gender Differences in Mate Selection: Evidence From a Speed Dating Experiment. You learned how to 
 
SELECT DISTINCT is used to return only distinct (different) values.


---
## Daily Happiness & Employee Turnover

```yaml
type: "TwoRowsWideTop"
key: "91a89ca986"
```

`@part1`
You learned:

- Difference types of JOINS

- Combining result sets with UNION and UNION ALL


`@part2`



`@part3`



`@script`



---
## Analysis of Refugee Crisis

```yaml
type: "TwoRowsWideTop"
key: "1fecb85d6d"
```

`@part1`



`@part2`



`@part3`



`@script`



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


