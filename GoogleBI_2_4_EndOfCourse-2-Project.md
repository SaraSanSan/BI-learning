# | The Path to Insights: DATA MODELS & PIPELINES |

# COURSE 2: END-OF-COURSE PROJECT

You’ll complete an end-of-course project by creating a pipeline process to deliver data to a target table and developing reports based on project needs. You’ll also ensure that the pipeline is performing correctly and that there are built-in defenses against data quality issues.

Learning Objectives:

    Identify business needs to determine a design for your portfolio project’s data pipeline.
    Analyze how database systems are designed, how to build BI tools such as pipelines and ETL systems, and how to optimize them to maximize performance to determine the most optimal data pipeline process.
    Develop a data pipeline to deliver necessary data to a target table.


## Welcome to module 4

Hi, it's great to be with you again!
I'm Anita,
a Senior Business Intelligence Analyst at Google,
and I'm back to discuss the next part
of your end-of-course project
and how you can use it in your job search.
Are you ready to start job searching
in the BI field?
The first step is to create a portfolio
and resume that exhibit your skills.
Your portfolio will be a collection
of materials that you can use to showcase
those skills and your approach
to solving BI problems.
One way you can build up your portfolio
is by completing projects that demonstrate
what you've learned –
like this program's end-of-course project!
This end-of-course project
is also a really valuable opportunity
to develop your interview skills!
As potential employers assess you as a candidate,
they might ask for specific examples
of how you have tackled challenges in the past.
You can use your portfolio as a way
to discuss real problems that you have solved.
Additionally, some employers might
ask you to complete another case study
for an interview.
Getting some practice creating
your own case studies means that
you'll be that much more prepared for those interviews.
You have already explored experiential learning,
or the idea of understanding through doing.
This end-of-course project
is also a great opportunity
to really discover how organizations
are using BI every day,
practice your new skills,
and really show off your BI knowledge.
In order to complete the end-of-course project,
you'll be presented with more details
about the business case.
Then, you'll use the key BI documents
you completed to create a pipeline system
that delivers data to reporting tables.
Later on, you can use these tables
to design dashboards to share insights with stakeholders.
By the time you complete this project,
you'll have a finished case study
you can add to your portfolio.
You'll also have documentation
of the steps you took along the way,
which you can use to explain
your work to future hiring managers.
At this point, you have probably already
completed one part of the end-of-course project.
Now, you're almost finished
with the next course of this program,
which means you know everything
you need to tackle the next phase.
Ready?
Then let's get started! 


# APPLY YOUR SKILLS TO A WORKPLACE SCENARIO

## Continue your end-of-course project

In this course, you've been learning about
how database systems are designed,
how to build BI tools such as pipelines and ETL systems,
and how to optimize them to maximize performance.
Now, it's time for an exciting next step:
putting all of this to work for your end-of-course project.
In the previous course,
you were introduced to the project scenario
and important details about the case.
Along the way, you developed Stakeholder Requirements,
Project Requirements, and Strategy Documents.
Now that you have
these important elements of the project laid out,
it's time to start thinking about the data.
In this part of the course,
you'll begin working with a database
in order to create BI tools that automate key processes
such as moving and transforming data
before reading it into your target tables for reporting.
Coming up, you're going to access the project data,
explore the design pattern for your database system,
observe your team's work to determine their needs,
and use required metrics and facts
to build a pipeline that meets those needs.
These processes will enable your team
to focus their time on
other aspects of their day-to-day jobs,
and will move and transform your data
for immediate use in reports and dashboards.
These reports and dashboards
will give your stakeholders updated insights
and empower them to get their own answers from the data.
This part of the end-of-course project
is a great opportunity to demonstrate to potential employers
that you can do exactly that.
And remember: developing these tools
is an iterative process,
so you can continue to build and improve them
as you have new ideas or learn new things. 


# CYCLISTIC SCENARIO

## Cyclistic datasets

By now, you’re getting ready to take the next steps with your Course 2 end-of-course project. To work with the Cyclistic project data, you will need to locate the appropriate public datasets and upload the zip code spreadsheet that your colleague shared into your BigQuery project space. This reading will guide you through that process. Once you have finished this reading, you will be ready for the upcoming activities and to deliver key insights to your stakeholders. 

For this end-of-course project, you will be using two public datasets, which exist in the public data available from the Explorer pane of your console: 

    NYC Citi Bike Trips
    Census Bureau US Boundaries
    GSOD from the National Oceanic and Atmospheric Administration

Additionally, you will need to upload the zip code spreadsheet your colleague shared with you. 

Upload to BigQuery: First, navigate to your BigQuery console. Go to the BigQuery homepage or navigate to the console.  

Search and preview the public datasets using the search bar in the Explore pane of your console:

These datasets are already available for you to query, but it can be useful to check out the tables before you start working with them. Find all three datasets by searching the appropriate dataset name in the search bar:

    new_york_citibike
    geo_us_boundaries
    noaa_gsod

After you have familiarized yourself with the public data, upload the zip code dataset. Either save the Google Sheet as a CSV file on your device or download it into your own Drive space. 

Click on the + ADD DATA button in the Explorer menu pane; this will open the Add Data menu. 

From here, select Local file to upload the CSV or Google Cloud Storage to choose the sheet from your personal Drive. However you add the file, you will need to fill out the necessary fields in the Create Table menu. If you haven’t already, the Create table menu will also prompt you to create a dataset to house this table.

Select CREATE NEW DATASET and name the dataset appropriately for this project. You can leave the data location set to default. Once you have completed filling out this information, click Create Dataset. 

Now, finish filling out the information for your table. Name your table appropriately for your project and select CSV under file type. Finally, select Auto detect for the schema. Once done, select Create Table. The new table should appear under your dataset in the Explorer pane momentarily. 

From here, explore the schema, preview the data, and familiarize yourself with this table. Once you have uploaded this dataset, you will be ready to continue with your project!


## Observe the Cyclistic team in action

Understanding your stakeholders and how they use the data is key to developing business intelligence solutions that will address their specific needs. In addition to meeting with stakeholders to discuss their project requirements, it can also be useful to observe the team at work and identify any patterns or frequently asked questions. 

In this reading, you’ll discover some of the ways that the Cyclistic team uses the data. This can inform the BI solution you develop for them and help you design the final reporting dashboard to be specific to their needs and useful to the whole team. As a BI professional, recognizing a team’s needs and customizing their systems can support their work as they make key business decisions. 

- The team at work

As you learned during your previous meeting with Cyclistic, the product development team has begun planning for the next year of Cyclistic’s bike-sharing program. Cyclistic's Customer Growth Team is creating a business plan for next year. The team wants to understand how their customers are using their bikes; their top priority is identifying customer demand at different station locations. The Cyclistic team posed an important primary question:

    How can we apply customer usage insights to inform new station growth?

Answering these questions starts with the data from the Cyclistic bikes themselves, which the team has provided you, and the reporting dashboard the team uses to gain insights. In addition to the explicit requests the stakeholders made, you realize a few key things about the team's current processes. 

First, you realize that there are stakeholders from a variety of different departments accessing and using this data with different levels of technical expertise. There are stakeholders from these teams:

    Product development
    Customer data
    Engineering
    Data analytics
    Data warehousing
    API
    IT
    Cyclistic executive
    Project management

For example, you realize that Earnest Cox, the VP of product development, is often requesting high-level insights into the data and rarely needs detailed overviews of the data. Alternatively, Tessa Blackwell from the data analytics team does explore the data in-depth and spends a lot more time reviewing the dashboard views. As you develop your reporting tools, you will want to find a way to answer both of these stakeholders’ needs. 

Additionally, one of your coworkers finds out you’re working on this project and shares a dataset they created recently for a project of their own that they think might help you: NYC zip codes. This dataset provides the zip codes for the different neighborhoods and boroughs in New York City; this will let you compare the bike data to the weather data more easily since you will be able to match the locations more accurately. It will also help you develop your map visualization later on.  

- Key takeaways

As you prepare to create the pipeline system that will deliver data to your reporting tables and eventually your dashboard, recognizing the different kinds of users, their specific needs and questions, and how they are currently using the data can help guide your development process. In this case, observing the Cyclistic team in action revealed that there are users who need different levels of detail and have different technical abilities. Additionally, you gained a useful tool from a colleague that will help you explore multiple datasets for this project. You can use these discoveries to design a BI solution that really addresses this organization’s unique needs–and demonstrate your skill and flexibility to future employers!


## CODE

For this activity, you could run the following SQL query to create a summary table for the entire year:

```
SELECT
TRI.usertype,
 ZIPSTART.zip_code AS zip_code_start,
 ZIPSTARTNAME.borough borough_start,
 ZIPSTARTNAME.neighborhood AS neighborhood_start,
  ZIPEND.zip_code AS zip_code_end,
  ZIPENDNAME.borough borough_end,
 ZIPENDNAME.neighborhood AS neighborhood_end,
  DATE_ADD(DATE(TRI.starttime), INTERVAL 5 YEAR) AS start_day,
  DATE_ADD(DATE(TRI.stoptime), INTERVAL 5 YEAR) AS stop_day,
  WEA.temp AS day_mean_temperature, -- Mean temp
 WEA.wdsp AS day_mean_wind_speed, -- Mean wind speed
  WEA.prcp day_total_precipitation, -- Total precipitation
 -- Group trips into 10 minute intervals to reduces the number of rows
  ROUND(CAST(TRI.tripduration / 60 AS INT64), -1) AS trip_minutes,
  COUNT(TRI.bikeid) AS trip_count
FROM
 `bigquery-public-data.new_york_citibike.citibike_trips` AS TRI
INNER JOIN
  `bigquery-public-data.geo_us_boundaries.zip_codes` ZIPSTART
 ON ST_WITHIN(
 ST_GEOGPOINT(TRI.start_station_longitude, TRI.start_station_latitude),
ZIPSTART.zip_code_geom)
INNER JOIN
  `bigquery-public-data.geo_us_boundaries.zip_codes` ZIPEND
  ON ST_WITHIN(
ST_GEOGPOINT(TRI.end_station_longitude, TRI.end_station_latitude),
ZIPEND.zip_code_geom)
INNER JOIN
`bigquery-public-data.noaa_gsod.gsod20*` AS WEA
  ON PARSE_DATE("%Y%m%d", CONCAT(WEA.year, WEA.mo, WEA.da)) = DATE(TRI.starttime)
INNER JOIN
  -- Note! Add your zip code table name, enclosed in backticks: `example_table`
  `(insert your table name) zipcodes` AS ZIPSTARTNAME
  ON ZIPSTART.zip_code = CAST(ZIPSTARTNAME.zip AS STRING)
INNER JOIN
  -- Note! Add your zipcode table name, enclosed in backticks: `example_table`
  `(insert your table name) zipcodes` AS ZIPENDNAME
  ON ZIPEND.zip_code = CAST(ZIPENDNAME.zip AS STRING)
WHERE
 -- This takes the weather data from one weather station
 WEA.wban = '94728' -- NEW YORK CENTRAL PARK
 -- Use data from 2014 and 2015
 AND EXTRACT(YEAR FROM DATE(TRI.starttime)) BETWEEN 2014 AND 2015
GROUP BY
 1, 
 2,
  3,
  4,
  5,
  6,
  7,
  8,
  9,
  10,
  11,
  12,
  13
```

The result of this query is a merged target table that JOINs the public datasets and the zip code table you uploaded. 

Additionally, you needed to execute a query that captured data from just the summer season:

```
SELECT
 TRI.usertype,
 TRI.start_station_longitude,
 TRI.start_station_latitude,
 TRI.end_station_longitude,
 TRI.end_station_latitude,
 ZIPSTART.zip_code AS zip_code_start,
 ZIPSTARTNAME.borough borough_start,
 ZIPSTARTNAME.neighborhood AS neighborhood_start,
 ZIPEND.zip_code AS zip_code_end,
  ZIPENDNAME.borough borough_end,
  ZIPENDNAME.neighborhood AS neighborhood_end,
 -- Since we're using trips from 2014 and 2015, we will add 5 years to make it look recent
  DATE_ADD(DATE(TRI.starttime), INTERVAL 5 YEAR) AS start_day,
 DATE_ADD(DATE(TRI.stoptime), INTERVAL 5 YEAR) AS stop_day,
  WEA.temp AS day_mean_temperature, -- Mean temp
 WEA.wdsp AS day_mean_wind_speed, -- Mean wind speed
  WEA.prcp day_total_precipitation, -- Total precipitation
  -- We will group trips into 10 minute intervals, which also reduces the number of rows
ROUND(CAST(TRI.tripduration / 60 AS INT64), -1) AS trip_minutes,
 TRI.bikeid
FROM  
 `bigquery-public-data.new_york_citibike.citibike_trips` AS TRI
INNER JOIN
`bigquery-public-data.geo_us_boundaries.zip_codes` ZIPSTART
ON ST_WITHIN(
ST_GEOGPOINT(TRI.start_station_longitude, TRI.start_station_latitude),
 ZIPSTART.zip_code_geom)
INNER JOIN
`bigquery-public-data.geo_us_boundaries.zip_codes` ZIPEND
ON ST_WITHIN(
 ST_GEOGPOINT(TRI.end_station_longitude, TRI.end_station_latitude),
ZIPEND.zip_code_geom)
INNER JOIN
 -- https://pantheon.corp.google.com/bigquery?p=bigquery-public-data&d=noaa_gsod
 `bigquery-public-data.noaa_gsod.gsod20*` AS WEA
 ON PARSE_DATE("%Y%m%d", CONCAT(WEA.year, WEA.mo, WEA.da)) = DATE(TRI.starttime)
INNER JOIN
-- Note! Add your zipcode table name, enclosed in backticks: `example_table`
`legalbi.sandbox.zipcodes` AS ZIPSTARTNAME
ON ZIPSTART.zip_code = CAST(ZIPSTARTNAME.zip AS STRING)
INNER JOIN
 -- Note! Add your zipcode table name below, enclosed in backticks: `example_table`
  `legalbi.sandbox.zipcodes` AS ZIPENDNAME
   ON ZIPEND.zip_code = CAST(ZIPENDNAME.zip AS STRING)
WHERE
-- Take the weather from one weather station
  WEA.wban = '94728' -- NEW YORK CENTRAL PARK
 -- Use data for three summer months
AND DATE(TRI.starttime) BETWEEN DATE('2015-07-01') AND DATE('2015-09-30')
```

This query results into a similar table as the previous query, except it focuses on trends from July through September. 

- Key takeaways

Storing data from multiple sources in target tables allows you to access and use consolidated data for reporting purposes. In the Course 3 end-of-course project, you will use the table you’ve created in this activity to design a dashboard and share insights with the Cyclistic product development team in order to help guide their process and make informed decisions.



# GOOGLE FIBER SCENARIO

## Google Fiber datasets

By now, you are getting ready to take the next steps with your Course 2 end-of-course project. To work with the Google Fiber data, you will need to upload your data to the appropriate workspace. If you plan on using BigQuery or Dataflow, upload the files to your project space to JOIN them. Additionally, because this data is already clean, you can connect these datasets in Tableau directly and merge them there. 

Your interviewers have provided three CSV files: 

    Market_1
    Market_2
    Market_3 

- Upload to BigQuery

First, navigate to your BigQuery console. Go to the BigQuery homepage or go directly to the console. 

Click on the + ADD DATA button in the Explorer menu pane to open the Add Data menu.

From here, select Local file to upload the CSV or Google Cloud Storage to choose the sheet from your personal Drive. However you add the file, you will need to fill out the necessary fields in the Create Table menu. If you haven’t already, the Create table menu will also prompt you to create a dataset to house this table.

Select CREATE NEW DATASET and name the dataset appropriately for this project. Leave the data location set to default. Once you have completed filling out this information, click Create Dataset. 

Now, finish filling out the information for your table. Name your table appropriately for your project and select CSV under file type. Finally, select Auto detect for the schema. Once done, select Create Table. The new table should appear under your dataset in the Explorer pane momentarily. 

From here, explore the schema, preview the data, and familiarize yourself with this table. Once you have uploaded this dataset, you will be ready to continue with your project!


## CODE

For this activity, you could run the following SQL query to create a single combined table that merged all three of the datasets your were given:

```
SELECT
  date_created,
  contacts_n,
  contacts_n_1,
  contacts_n_2,
  contacts_n_3,
  contacts_n_4,
  contacts_n_5,
  contacts_n_6,
  contacts_n_7,
  new_type,
  new_market
FROM `your project.fiber.market_1`
UNION ALL
SELECT
  date_created,
  contacts_n,
  contacts_n_1,
  contacts_n_2,
  contacts_n_3,
  contacts_n_4,
  contacts_n_5,
  contacts_n_6,
  contacts_n_7,
  new_type,
  new_market
FROM `your project.fiber.market_2`
UNION ALL
SELECT
  date_created,
  contacts_n,
  contacts_n_1,
  contacts_n_2,
  contacts_n_3,
  contacts_n_4,
  contacts_n_5,
  contacts_n_6,
  contacts_n_7,
  new_type,
  new_market
FROM `your project.market_3`
```

The UNION ALL statement is applied here instead of a JOIN statement because the tables already have matching columns, making them easy to merge completely. 

After you have run this query, you should have a combined table.

- Key takeaways

Storing data from multiple sources in target tables allows you to access and use consolidated data for reporting purposes. In the Course 3 end-of-course project, you will use the table you’ve created in this activity to design a dashboard and share insights with the Google Fiber stakeholders in order to help guide their process and make informed decisions.



# END-OF-COURSE PROJECT WRAP-UP

## Tips for ongoing success with your end-of-course project

At this point in your end-of-course project,
you've done a lot of work already.
You collaborated with stakeholders to determine their needs
and create important project planning documents;
then you used those to explore the project data
and build systems to deliver the data.
As you continue to work on your end-of-course project,
you'll want to consider how you can highlight your process
and explain what you've done
to potential employers and hiring managers.
First, it's important to recognize that,
as a BI professional,
you may be asked to learn and adapt to new tools.
There are a lot of great solutions out there,
and different businesses use different BI tools
depending on their needs.
Keep in mind that you have learned a lot
of transferrable skills that can be applied
across different tools.
You've also learned the importance of understanding
and observing how stakeholders can use data
in order to better meet their data needs;
you recognize the different types of databases
and storage systems and how they can be useful
in a larger database system; and you understand the logic
behind pipelines that ingest, transform, and deliver data.
These are all skills worth highlighting in job interviews,
no matter what tools the position requires.
In addition, always be sure to consider your audience.
As you have been learning throughout these courses,
you will often work with different kinds of stakeholders
who have different levels of technical know-how.
When you communicate with them,
keep in mind who they are and what their goals are,
and what they already know and what they need to know.
This is just as true when you're discussing
your end-of-course project with interviewers.
Often, there will be people conducting
or joining your interview
who aren't necessarily BI professionals.
For example, hiring managers may not have
the same detailed understanding of BI processes as you do.
In order to keep your presentation relevant to them,
try to remember those key questions about your audience.
Your interviewers have a business challenge,
just like stakeholders on a BI project:
They have an open job position to fill.
Think about what they need to know about you
that makes a decision that solves that.
Coming up, you're going to learn all about
presenting BI insights to your stakeholders
and providing them with access to relevant data
they can use to make decisions.
By the end of these courses,
you'll wrap up your end-of-course project
by creating dashboards and presentations.
In no time, you'll have a complete case study
for your portfolio. 


## Luis: Tips for interview preparation

My name is Luis and I'm a data and analytics manager at google.
When I'm preparing for an interview, I like to prepare a document where
I describe what is the role, What are the typical questions and
the typical type of interviews that this company does,
What is the team or the organization this role I'm applying for?
What are the projects that help this team to grow and and
to Excel and also to prepare the technical side of it.
So prepare the portfolio, understand the impact that I want to
showcase what is aligned with the company's strategy and
really take the time at least two weeks to really be ready for a first interview.
A portfolio is a collection of your past experience and the past projects
that you think are useful to showcase to someone that is interviewing you.
It's basically your brand and
you need to make sure that the project showcase the value of your brand.
The common mistake that I usually see is
the lack of showcasing impact on the technical side,
ensure that you understand why you created a data solution.
What was the outcome?
What is the impact?
How did you measure that on top of that?
Make sure that you also are capable of explaining why you
applied a certain solution instead of others and
also make sure that you define and you are able to explain the next steps,
what can be done on top of this solution when you are preparing for
an interview, make sure that you rehearse the interview with someone else.
It's important that you make sure that you are able to, you tell the right message
that you focus on impact that you are able to sell yourself the best way you can.
So you need to be really prepared for the interview and
rehearsing with someone that you trust that you are comfortable with receiving
feedback is really key to make you ready to answer the interview questions.
If B. I.
Is really the path that you want to pursue,
this is the very good first step to take into it.
But you should not stop here, go out and talk with people.
There are multiple meetups that happen around data around BI,
so don't feel that you are alone on this on this road.
There are multiple people that can help you increase your network, make
connections you'll be able to share and you also receive knowledge from others. 



# COURSE 2 REVIEW

## Course wrap-up

Congratulations on completing another course.
You're that much closer to finishing
this program and receiving your certificate.
You've learned a lot already.
Take a moment to consider everything
we've covered in this course and celebrate.
For example, you learned about database modeling,
design patterns, and how to use
database schema to describe those design patterns.
You also discovered many kinds of
databases and how they have
different uses within a database system.
Next, you explore data pipelines
and how ETL and ELT processes
help get data where it needs to go and
transform it to be useful during that process.
You also learned about different data storage systems
that you might use in a pipeline.
Additionally, you explored more common BI tools
and how to interact with stakeholders effectively.
You even had a chance to create your own pipeline.
Then by exploring database and pipeline optimization,
you were able to consider how BI
processes and systems are often iterative.
Coming up, you have
even more exciting discoveries to make.
Now that you understand how to create
systems to deliver data to stakeholders,
it's time to start thinking about how to present
that data and make it
accessible and useful for decision-making.
In the next course, you're going to
learn more about how to design
visualizations and dashboards for
BI and present those insights.
Great work so far. 


## Get started on Course 3

Congratulations on completing another course in the Google Business Intelligence Certificate! In this part of the program, you learned more about data modeling and ETL processes for extracting data from source systems, and transforming it into formats that better enable analysis and drive business processes and goals.

The entire program has three courses: 

1. Foundations of Business Intelligence: In this course, you will discover the role of business intelligence professionals within an organization, as well as typical career paths. You will explore core BI practices and tools and how BI professionals use them to make an impact.

2. The Path to Insights: Data Models and Pipelines: This is the course you’ve just completed. 

3. Decisions, Decisions: Dashboards and Reports: In this course, you will apply your knowledge of business intelligence and data modeling to create dynamic dashboards that track KPIs to meet stakeholder needs.


## GLOSSARY

A
Accuracy: An element of quality testing used to confirm that data conforms to the actual entity
being measured or described
Application programming interface (API): A set of functions and procedures that integrate
computer programs, forming a connection that enables them to communicate
Applications software developer: A person who designs computer or mobile applications,
generally for consumers
Attribute: In a dimensional model, a characteristic or quality used to describe a dimension

B
Business intelligence (BI): Automating processes and information channels in order to
transform relevant data into actionable insights that are easily available to decision-makers
Business intelligence governance: A process for defining and implementing business
intelligence systems and frameworks within an organization
Business intelligence monitoring: Building and using hardware and software tools to easily
and rapidly analyze data and enable stakeholders to make impactful business decisions
Business intelligence stages: The sequence of stages that determine both BI business value
and organizational data maturity, which are capture, analyze, and monitor
Business intelligence strategy: The management of the people, processes, and tools used in
the business intelligence process
Business rule: A statement that creates a restriction on specific parts of a database

C
Columnar database: A database organized by columns instead of rows
Combined systems: Database systems that store and analyze data in the same place
Compiled programming language: A programming language that compiles coded instructions that are executed directly by the target machine
Completeness: An element of quality testing used to confirm that data contains all desired components or measures
Conformity: An element of quality testing used to confirm that data fits the required destination format
Consistency: An element of quality testing used to confirm that data is compatible and in
agreement across all systems
Contention: When two or more components attempt to use a single resource in a conflicting way

D
Data analysts: People who collect, transform, and organize data
Data availability: The degree or extent to which timely and relevant information is readily
accessible and able to be put to use
Data dictionary: A collection of information that describes the content, format, and structure of
data objects within a database, as well as their relationships
Data governance professionals: People who are responsible for the formal management of
an organization’s data assets
Data integrity: The accuracy, completeness, consistency, and trustworthiness of data
throughout its life cycle
Data lake: A database system that stores large amounts of raw data in its original format until
it’s needed
Data lineage: The process of identifying the origin of data, where it has moved throughout the
system, and how it has transformed over time
Data mapping: The process of matching fields from one data source to another
Data mart: A subject-oriented database that can be a subset of a larger data warehouse
Data maturity: The extent to which an organization is able to effectively use its data in order to
extract actionable insights
Data model: A tool for organizing data elements and how they relate to one another
Data partitioning: The process of dividing a database into distinct, logical parts in order to
improve query processing and increase manageability
Data pipeline: A series of processes that transports data from different sources to their final
destination for storage and analysis
Data visibility: The degree or extent to which information can be identified, monitored, and
integrated from disparate internal and external sources
Data warehouse: A specific type of database that consolidates data from multiple source
systems for data consistency, accuracy, and efficient access
Data warehousing specialists: People who develop processes and procedures to effectively
store and organize data
Database migration: Moving data from one source platform to another target database
Database performance: A measure of the workload that can be processed by a database, as
well as associated costs
Deliverable: Any product, service, or result that must be achieved in order to complete a project
Developer: A person who uses programming languages to create, execute, test, and
troubleshoot software applications
Dimension (data modeling): A piece of information that provides more detail and context
regarding a fact
Dimension table: The table where the attributes of the dimensions of a fact are stored
Design pattern: A solution that uses relevant measures and facts to create a model in support
of business needs
Dimensional model: A type of relational model that has been optimized to quickly retrieve data
from a data warehouse
Distributed database: A collection of data systems distributed across multiple physical
locations

E
ELT (extract, load, and transform): A type of data pipeline that enables data to be gathered
from data lakes, loaded into a unified destination system, and transformed into a useful format
ETL (extract, transform, and load): A type of data pipeline that enables data to be gathered
from source systems, converted into a useful format, and brought into a data warehouse or
other unified destination system
Experiential learning: Understanding through doing

F
Fact: In a dimensional model, a measurement or metric
Fact table: A table that contains measurements or metrics related to a particular event
Foreign key: A field within a database table that is a primary key in another table (Refer to
primary key)
Fragmented data: Data that is broken up into many pieces that are not stored together, often
as a result of using the data frequently or creating, deleting, or modifying files
Functional programming language: A programming language modeled around functions

G
Google DataFlow: A serverless data-processing service that reads data from the source,
transforms it, and writes it in the destination location

I
Index: An organizational tag used to quickly locate data within a database system
Information technology professionals: People who test, install, repair, upgrade, and maintain
hardware and software solutions
Integrity: An element of quality testing used to confirm that data is accurate, complete,
consistent, and trustworthy throughout its life cycle
Interpreted programming language: A programming language that uses an interpreter,
typically another program, to read and execute coded instructions
Iteration: Repeating a procedure over and over again in order to keep getting closer to the
desired result

K
Key performance indicator (KPI): A quantifiable value, closely linked to business strategy,
which is used to track progress toward a goal

L
Logical data modeling: Representing different tables in the physical data model

M
Metric: A single, quantifiable data point that is used to evaluate performance

O
Object-oriented programming language: A programming language modeled around data
objects
OLAP (Online Analytical Processing) system: A tool that has been optimized for analysis in
addition to processing and can analyze data from multiple databases
OLTP (Online Transaction Processing) database: A type of database that has been
optimized for data processing instead of analysis
Optimization: Maximizing the speed and efficiency with which data is retrieved in order to
ensure high levels of database performance

P
Portfolio: A collection of materials that can be shared with potential employers
Primary key: An identifier in a database that references a column or a group of columns in
which each row uniquely identifies each record in the table (Refer to foreign key)
Project manager: A person who handles a project’s day-to-day steps, scope, schedule, budget,
and resources
Project sponsor: A person who has overall accountability for a project and establishes the
criteria for its success
Python: A general purpose programming language

Q
Quality testing: The process of checking data for defects in order to prevent system failures; it
involves the seven validation elements of completeness, consistency, conformity, accuracy,
redundancy, integrity, and timeliness
Query plan: A description of the steps a database system takes in order to execute a query

R
Redundancy: An element of quality testing used to confirm that no more data than necessary is
moved, transformed, or stored
Resources: The hardware and software tools available for use in a database system
Response time: The time it takes for a database to complete a user request
Row-based database: A database that is organized by rows

S
Schema validation: A process to ensure that the source system data schema matches the
target database data schema
Separated storage and computing systems: Databases where data is stored remotely, and
relevant data is stored locally for analysis
Single-homed database: Database where all of the data is stored in the same physical location
Snowflake schema: An extension of a star schema with additional dimensions and, often,
subdimensions
Star schema: A schema consisting of one fact table that references any number of dimension
tables
Strategy: A plan for achieving a goal or arriving at a desired future state
Subject-oriented: Associated with specific areas or departments of a business
Systems analyst: A person who identifies ways to design, implement, and advance information
systems in order to ensure that they help make it possible to achieve business goals
Systems software developer: A person who develops applications and programs for the
backend processing systems used in organizations

T
Tactic: A method used to enable an accomplishment
Target table: The predetermined location where pipeline data is sent in order to be acted on
Throughput: The overall capability of the database’s hardware and software to process
requests
Timeliness: An element of quality testing used to confirm that data is current
Transferable skill: A capability or proficiency that can be applied from one job to another

V
Vanity metric: Data points that are intended to impress others, but are not indicative of actual
performance and, therefore, cannot reveal any meaningful business insights

W
Workload: The combination of transactions, queries, data warehousing analysis, and system
commands being processed by the database system at any given time
