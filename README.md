# Project Overview

In this project, i used SQL to explore a database related to movie rentals. I wrote SQL code to run SQL queries and built visualizations to showcase the output of the queries in order to answer interesting questions about the database.

# Project Details

In this project, I queried the Sakila DVD Rental database. The Sakila Database holds information about a company that rents movie DVDs.

For this project, i queried the database to gain an understanding of the customer base, such as what the patterns in movie watching are across different customer groups, how they compare on payment earnings, and how the stores compare in their performance. The schema for the DVD Rental database is provided by link below. Source: http://www.postgresqltutorial.com/postgresql-sample-database/

# How to run this project : local environment

You can run the queries on your local machine using a database system, PostgreSQL. PostgreSQL is an open-source object-relational database system that is used frequently in industry. Hence, you may find learning to set up a PostgreSQL database on your local machine involves a sharp learning curve. You will have two additional tasks to complete:

* You will need to install the database system, PostgreSQL.

Select the following three components during installation - PostgreSQL server, pgAdmin, and command-line tools. pgAdmin is a GUI tool for managing the database. Download the installer from the link below, and install with the admin privileges:

- Installing PostgreSQL for Windows:

https://www.postgresql.org/download/windows/ and follow the steps mentioned https://www.postgresqltutorial.com/install-postgresql/

- Installing PostgreSQL for Mac OS:

https://www.postgresql.org/download/macosx/ and follow the steps mentioned https://www.postgresqltutorial.com/install-postgresql-macos/

* You will need to load the database in your local PostgreSQL database server.
Once PostgreSQL server is installed, you will need to download the Movie database from this page:https://www.postgresqltutorial.com/postgresql-sample-database/

# Understanding the Database

* To understand this database, you need to know :

- content and how many foreign keys in each tables

- start with creating a table that provides the following details: actor's first and last name combined as full_name, film title, film description and length of the movie. How many rows are there in the table?

- Write a query that captures the actor id, full name of the actor, and counts the number of movies each actor has made. Identify the actor who has made the maximum number movies ?

- Write a query that creates a list of actors and movies where the movie length was more than 60 minutes. How many rows are there in this query result?

- Write a query that displays a table with 4 columns: actor's full name, film title, length of movie, and a column name "filmlen_groups" that classifies movies based on their length. Filmlen_groups should include 4 categories: 1 hour or less, Between 1-2 hours, Between 2-3 hours, More than 3 hours.

# What are the Question Sets?
In this project, I answered  a set of questions that you are free to consider and you can try to answer another questions in your choice.

- Question 1 : We want to understand more about the movies that families are watching. The following categories are considered family movies: Animation, Children, Classics, Comedy, Family and Music.

Create a query that lists each movie, the film category it is classified in, and the number of times it has been rented out.

HINT: One way to solve this is to create a count of movies using aggregations, subqueries and Window functions.

- Question 2 : Now we need to know how the length of rental duration of these family-friendly movies compares to the duration that all movies are rented for.

Can you provide a table with the movie titles and divide them into 4 levels (first_quarter, second_quarter, third_quarter, and final_quarter) based on the quartiles (25%, 50%, 75%) of the rental duration for movies across all categories? Make sure to also indicate the category that these family-friendly movies fall into.

HINT: One way to solve it requires the use of percentiles, Window functions, subqueries or temporary tables.

- Question 3 :Provide a table with the family-friendly film category, each of the quartiles, and the corresponding count of movies within each combination of film category for each corresponding rental duration category. The resulting table should have three columns: Category, Rental length category, and Count

HINT: One way to solve this question requires the use of Percentiles, Window functions and Case statements.

- Question 4 : We want to find out how the two stores compare in their count of rental orders during every month for all the years we have data for.

HINT: One way to solve this query is the use of aggregations.

- Question 5 : We would like to know who were our top 10 paying customers, how many payments they made on a monthly basis during 2007, and what was the amount of the monthly payments.

HINT: One way to solve is to use a subquery, limit within the subquery, and use concatenation to generate the customer name.

- Question 6 : Finally, for each of these top 10 paying customers, I would like to find out the difference across their monthly payments during 2007.

HINT: You can build on the previous questions query to add Window functions and aggregations to get the solution.

# Data visualizations & queries
In order to create the data visualizations for some interesting question above, i exported the results of my queries from the Project Workspace (PostgreSQL).I moved the data out of my PostgreSQL and into Python (import matplotlib.pyplot as plt) or another spreadsheet application like Excel, Google Sheets.

# Extra link to helped me solve this project

- https://matplotlib.org/stable/gallery/lines_bars_and_markers/barchart.html#sphx-glr-gallery-lines-bars-and-markers-barchart-py

- https://mode.com/sql-tutorial/sql-business-analytics-training/

- https://www.python.org/dev/peps/pep-0008/#tabs-or-spaces

- https://www.postgresql.org/docs/8.4/functions-window.html

- https://www.postgresql.org/docs/9.1/tutorial-window.html

- https://docs.actian.com/ingres/10.2/index.html#page/SQLRef%2FRegression_and_Correlation_Analysis_Aggregate_Fu.htm%23

- https://www.techonthenet.com/sql/union.php

- https://www.hackerrank.com/domains/sql

- https://www.analyticsvidhya.com/blog/2017/01/46-questions-on-sql-to-test-a-data-science-professional-skilltest-solution/
