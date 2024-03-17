# [MScBA Business Analytics & Management student @ RSM :link:](https://www.rsm.nl/education/master/msc-programmes/mscba-business-analytics-management/)

## Projects

### Data Management with SQL using 'InsideAirbnb'

Tools: SQLite, DB Browser for SQLite, LaTeX (reporting)

Data: [InsideAirbnb](http://insideairbnb.com/) London dataset

Find the full report [here](projects/sql/sql_report.pdf).

Find the full code [here](projects/sql/sql_code.txt).

#### Intro

While "shared economy" business models arose and were positioned as the cheaper alternatives to hotels that benefit individuals, with years it has developed into a professional marketplace. In this project I investigated the severity of Airbnb presence in London on its' citizens. Given the current housing crisis, I was interested in seeing how the hosts developed their listings portfolio and how those could affect the scarcity in the property market in London.

In the report, I posed these questions regarding the London Airbnb market:

- What is the average number of listings per host based on the year of joining the Airbnb platform?
- What is the number of listings for all neighbourhoods for the biggest host?

#### Implementation

To achieve that, a two-step The first part involved wrangling the original data from InsideAirbnb (using SQL). Some of the processes involved:

- Checking for duplicated data
- Handling of the missing values: resolved by imputation (due to low number of missing values)
- Outliers analysis
- Date formatting
- Spelling errors

The second part of the project involved implementing the database in line with normalization principles, as shown below, as well as the querying required to answer the research questions.

![Entity Relationship Diagram](projects/sql/ERD.png)

#### Results

For the first question, the following visualization was made:

![Line plot of average # of listings per year of joining](projects/sql/Q1.png)

Two interesting patterns arise:

1. For the hosts who joined between 2010 and 2016, the number of listings is relatively low. At that time, Airbnb was booming in popularity, but people still used it as intended.
2. For the hosts who joined after 2016, the later the hosts were joining the platform, the more listings they had on average. Based on that finding, I argue that the intention of new hosts on the platform was to generate additional income by investing and renting the properties in a short-term.

For the second question, I found the following:

![Line plot of average # of listings per year of joining](projects/sql/Q3.png)

Westminster, as a central location in London, is clearly favoured over other neighbourhoods. Easy access to tourist attractions, as well as great connection to many other parts of London makes this district a prime location for short-term property rental. Interestingly, Brent was the second biggest neighbour in terms of nubmer of listings offered by the biggest host. Perhaps the good transport connection to other parts of London, as well as the Wembley Stadium could explain why this area is of an interest to professional Airbnb hosts.

### Process mining for an insurance company using Celonis

Tools: Celonis, Python

For the Business Analytics Workshop course during my master, I was a part of the team responsible for bringing insights for the dutch insurance firm using process mining. The company wanted to understand better how fast are their processes related to clients executed.

As a part of this project, I had to learn the theory behind process mining. Some of the key aspects of that involved:

- Process discovery: transforming the event log into process model
- Conformance checking: comparing the *de facto* model against the firm expectations
- Performance analysis: analysing the duration of the processes, rework, definition of happy / unhappy flows

Additionally, during the project I learned how to use **Celonis**. More specifically, I was responsible for:

- Configuring the data model consisting of multiple tables
- Developing dashboards
- Redefining KPI's, e.g.: rework

Thanks to the use of additional data sets, I was able to expand the scope of analysis with client-specific information, allowing more depth in understanding the processes.

*Side note*: Initially the goal was to perform the analysis using Python's **PM4PY** library. However, it very quickly became clear that Celonis provides better quality of analysis. Use of dashboards and dynamic filtering, similar to PowerBi / Tableau, is more intuitive to end user of the analysis than the implementation of process mining in Python.

### Predicting number of enrolled students at the university

