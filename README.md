<img src="https://raw.githubusercontent.com/codecaviar/digital_asset_management/master/assets/bingyune-and-company-logo-6400x3600.png" align="left" width="200" height="auto">

<br/><br/><br/><br/>

----------

# Bike Share for All: Complete Guide to Intermediate SQL

**Code Caviar Story**: https://www.bingyune.com/blog/bike-share-intermediate-sql

## Project Overview

Databases impact our everyday lives in some shape or form (often without us even being aware of it). Take coffee, as an example. Each time you buy a pumpkin spice latte, you scan your rewards card and earn rewards points that you can redeem later towards the purchase of more lattes. All of that purchase and rewards information then gets stored in a database. Fortunately, SQL can help us rapidly navigate these databases - query, retrieve, and aggregate millions of records to gain insights. SQL programming can be used to insert, search, update, and delete database records. It can also do things such as optimize and maintain databases. Even with the expansion of "Not Only SQL" or NoSQL databases, there's still no need to become unnecessarily distracted by the shiny, new-fangled, NoSQL red button just yet. Traditional, relational databases are cornerstones of data ecosystems, making SQL the most popular standard query language to access data. When you are able to understand SQL and use it effectively, you will be able to harness even more powerful features and technologies in the data industry.

**The goal of this project is** to provide a Complete Guide to the intermediate hacking skills needed to aggregate data across entire columns or merge multiple datasets together with SQL. The project makes use of the [Bay Area Bike Share](https://mtc.ca.gov/our-work/operate-coordinate/traveler-services/bay-area-bike-share) data sourced from [Kaggle](https://www.kaggle.com/benhamner/sf-bay-area-bike-share). The original dataset contains data for 70 stations (where users can pickup or return bikes), about 71M status updates (number of bikes and docks available for given station), about 670k trips (individual bike trips), and about 3k weather forecasts (for a specific day for a certain zip code).

## Summary:

Up until now, you may have only been working with one SQL table at a time so far. However, the real power of SQL comes from working with data from multiple tables at once. A SQL database is also called a "relational database" because the tables within the database "relate" to one another through common unique identifiers (keys). The relationship between tables allows information from multiple tables to be combined easily in SQL. There are two main approaches to combining information from multiple tables:

* `UNION` merges rows of similar data to create a new set, essentially stacking one table on top of another.
* `JOIN` combines columns from tables using common unique identifiers (keys).

There are also many SQL aggregate functions that can be used to aggregate your data, such as `MIN`, `MAX`, `SUM`, `AVG`, and `COUNT`. It's important to remember that aggregations only aggregate vertically in a particular column. A few valuable SQL clauses that are often used with aggregations are `GROUP BY` and `HAVING`.

In the [Beginner's Guide to Basic SQL](https://www.bingyune.com/blog/bike-share-basic-sql), many of the practice problems could only be solved in one or two ways with the skills you learned. As you progress and problems get harder, there will be many ways of producing the correct results. Keep in mind that the answers to practice problems should be used as a reference, but are by no means the only ways of answering the questions. Here are a few ways to validate your query results:

* Check that the table and column names are correct
* Check that your single quotes ( `‘` ) or double quotes ( `“` ) are closed
* Check operators such as `>`, `<`, `=`, `!=`, etc.
* Use [`EXPLAIN`](https://sqlite.org/lang_explain.html) before `SELECT` to check how your SQL statement will access your database
* Review error messages when your query does not run
* Apply business context or industry knowledge (of similar data) to check the order of magnitude

## Getting Started

First, cloning the git repository and installing the provided packages will help you get a copy of the project up and running on your local machine. The project was created using Jupyter Notebook (.ipynb) and the packages were managed using the Anaconda platform.

```
git clone https://github.com/codecaviar/bike_share_intermediate_sql.git
conda env create -f environment.yml
```

File Description:
* environment.yml - packages used to perform this analysis
* notebook_bike_share_intermediate_sql.ipynb - Jupyter Notebook for this project including code examples and explanations
* solutions_bike_share_intermediate_sql.ipynb - Jupyter Notebook for this project including solutions to practice problems

## Authors

- **BingYune Chen** - [LinkedIn](https://www.linkedin.com/in/bingyune-chen/)
- **BingYune & Co** - [GitHub](https://github.com/codecaviar)

## License

The project is licensed under the GNU General Public License v3.0 License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

The project referenced the following resources:
* https://mode.com/sql-tutorial/
* https://www.w3schools.com/sql/
* https://www.sqlitetutorial.net/

----------
The Code Caviar is a digital magazine about data science and analytics that dives deep into key topics, so you can experience the thrill of solving at scale.
