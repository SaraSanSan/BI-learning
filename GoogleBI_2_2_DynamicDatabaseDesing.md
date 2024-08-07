# | The Path to Insights: DATA MODELS & PIPELINES |

# DYNAMIC DATABASE DESING

You’ll learn more about database systems, including data marts, data lakes, data warehouses, and ETL processes. You’ll also investigate the five factors of database performance: workload, throughput, resources, optimization, and contention. Finally, you’ll consider how to design efficient queries that get the most from a system.

Learning Objectives:

    Discover strategies to create an ETL process that works to meet organizational and stakeholder needs and maintain an ETL process efficiently.
    Understand what the different data storage and extraction processes and tools may include (Extract/L: Stitch/Segment/Fivetran, Transform: DBT/Airflow/Looker).
    Explain how to optimize when building new tables.
    Identify and describe where new tables can fit in the pipeline.
    Recognize the different aspects of databases, including OLAP and OLTP, columnar and relational, distributed and single-homed databases.
    Understand the importance of database performance and optimization.
    Describe the different five factors of database performance: workload, throughput, resources, optimization, and contention.
    Perform pipeline debugging using queries.


## Welcome to module 2

In order to efficiently deliver the most up to date information to your
stakeholders,
you must first understand and optimize query performance within your pipelines.
And that's we're going to explore the next few videos.
We'll discover how to increase throughput and minimize the competition for
resources within the system to enable the largest possible workload to be processed.
We'll get into database systems including data marts,
data lakes, data warehouses and ELT processes.
That's not a typo, ELT is different from ETL.
It stands for extract, load and transform.
You'll also witness how these systems contribute to the overall efficiency of
your data systems.
In addition, you'll investigate the five factors of database performance,
workload, throughput, resources, optimization and contention.
And you'll gain some tips for making sure your database intake and
storage are the best they can be.
Finally, we'll begin thinking about how to design efficient queries that really get
the most out of your systems.
Let's do it. 



# DATABASE PERFORMANCE

## Data marts, data lakes, and the ETL process

One of the amazing things about BI, is that the tools and
processes are constantly evolving.
Which means BI professionals always have new opportunities to build and
improve current systems.
So, let's learn about some other interesting data storage and
processing patterns you might encounter as a BI professional.
Throughout these courses, we've learned about database systems that make use of
data warehouses for their storage needs.
As a refresher, a data warehouse is a specific type of database that
consolidates data from multiple source systems for data consistency,
accuracy and efficient access. 

Basically, a data warehouse is a huge collection of data from all the company's
systems.
Data warehouses were really common when companies used a single machine,
to store and compute their relational databases.
However, with the rise of cloud technologies and explosion of data volume,
new patterns for data storage and computation emerged.
One of these tools is a data mart, as you may recall a data mart is a subject
oriented database that can be a subset of a larger data warehouse.
NBI, subject oriented, describes something that is associated with specific areas or
departments of a business such as finance, sales or marketing.
As you're learning, BI projects commonly focus on answering various questions for
different teams.
So a data mart is a convenient way to access the relevant data that needs to be
pulled for a particular project.
Now, let's check out data lakes.
A data lake is a database system that stores large amounts of raw data
in its original format until it's needed.
This makes the data easily accessible,
because it doesn't require a lot of processing.
Like a data warehouse, a data lake combines many different sources, but
data warehouses are hierarchical with files and folders to organize the data.
Whereas data lakes are flat and while data has been tagged so it is identifiable,
it's not organized, it's fluid, which is why it's called a data lake.
Data lakes don't require the data to be transformed before storage.
So they are useful if your BI system is ingesting a lot of different data types.
But of course, the state eventually needs to get organized and transformed.
One way to integrate data lakes into a data system is through ELT
previously we learned about the ETL process,
where data is extracted from the source into the pipeline.
Transformed, while it is being transported and then loaded into its destination.
ELT takes the same steps but reorganizes them so
that the pipeline Extracts, Loads and then Transforms the data.
Basically ELT is a type of data pipeline that enables data to be gathered from
different sources.
Usually data lakes, then loaded into a unified destination system and
transformed into a useful format.
ELT enables BI professionals to ingest so many different kinds of data into
a storage system as soon as that data is available.
And they only have to transform the data they need, ELT also reduces storage costs
and enables businesses to scale storage and computation resources independently.
As technology advances,
the processes and tools available also advance and that's great.
Some of the most successful BI professionals do well because they
are curious lifelong learners. 


## ETL versus ELT

So far in this course, you have learned about ETL pipelines that extract, transform, and load data between database storage systems. You have also started learning about newer pipeline systems like ELT pipelines that extract, load, and then transform data. In this reading, you are going to learn more about the differences between these two systems and the ways different types of database storage fit into those systems. Understanding these differences will help you make key decisions that promote performance and optimization to ensure that your organization’s systems are efficient and effective.

The primary difference between these two pipeline systems is the order in which they transform and load data. There are also some other key differences in how they are constructed and used.

### DIFFERENCES ETL VS ELT

The order of extraction, transformation, and loading data:

    ETL: Data is extracted, transformed in a staging area, and loaded into the target system
    ELT: Data is extracted, loaded into the target system, and transformed as needed for analysis

Location of transformations:

    ETL: Data is moved to a staging area where it is transformed before delivery
    ELT: Data is transformed in the destination system, so no staging area is required

Age of the technology:

    ETL: ETL has been used for over 20 years, and many tools have been developed to support ETL pipeline systems
    ELT: ELT is a newer technology with fewer support tools built-in to existing technology

Access to data within the system:

    ETL: ETL systems only transform and load the data designated when the warehouse and pipeline are constructed
    ELT: ELT systems load all of the data, allowing users to choose which data to analyze at any time

Calculations

    ETL: Calculations executed in an ETL system replace or revise existing columns in order to push the results to the target table
    ELT: Calculations are added directly to the existing dataset

Compatible storage systems

    ETL: ETL systems are typically integrated with structured, relational data warehouses
    ELT: ELT systems can ingest unstructured data from sources like data lakes

Security and compliance

    ETL: Sensitive information can be redacted or anonymized before loading it into the data warehouse, which protects data
    ELT: Data has to be uploaded before data can be anonymized, making it more vulnerable

Data size

    ETL: ETL is great for dealing with smaller datasets that need to undergo complex transformations
    ELT: ELT is well-suited to systems using large amounts of both structured and unstructured data

Wait times

    ETL: ETL systems have longer load times, but analysis is faster because data has already been transformed when users access it
    ELT: Data loading is very fast in ELT systems because data can be ingested without waiting for transformations to occur, but analysis is slower

### Data storage systems

Because ETL and ELT systems deal with data in slightly different ways, they are optimized to work with different data storage systems. Specifically, you might encounter data warehouses and data lakes. As a refresher, a data warehouse is a type of database that consolidates data from multiple source systems for data consistency, accuracy, and efficient access. And a data lake is a database system that stores large amounts of raw data in its original format until it’s needed. While these two systems perform the same basic function, there are some key differences:

Data processed ?

    Data warehouse: Data has already been processed and stored in a relational system
    Data lake: Data is raw and unprocessed until it is needed for analysis; additionally, it can have a copy of the entire OLTP or relational database

Data purpose ?

    Data warehouse: The data’s purpose has already been assigned, and the data is currently in use
    Data lake: The data’s purpose has not been determined yet

Data adaptability ?

    Data warehouse: Making changes to the system can be complicated and require a lot of work
    Data lake: Systems are highly accessible and easy to update

There is also a specific type of data warehouse you might use as a data source: data marts. Data marts are very similar to data warehouses in how they are designed, except that they are much smaller. Usually, a data mart is a single subset of a data warehouse that covers data about a single subject.

- Key takeaways:

Currently, ETL systems that extract, transform and load data, and ELT systems that extract, load, and then transform data are common ways that pipeline systems are constructed to move data where it needs to go. Understanding the differences between these systems can help you recognize when you might want to implement one or the other. And, as business and technology change, there will be a lot of opportunities to engineer new solutions using these data systems to solve business problems.


## The five factors of database performance

We've been investigating database optimization
and why it's important to make
sure that users are able to get what they
need from the system as efficiently as possible.
Successful optimization can be
measured by the database performance.
Database performance is a measure of
the workload that can be processed by a database,
as well as the associated costs.
In this video, we're going to consider
the factors that influence database performance,
workload, throughput,
resources, optimization, and contention.
First, we'll start with workload.
In BI, workload refers to
the combination of transactions, queries,
analysis, and system commands being
processed by the database system at any given time.
It's common for a database's workload to
fluctuate drastically from day to day,
depending on what jobs are being processed
and how many users are interacting with the database.
The good news is that you can
often predict these fluctuations.
For instance, there might be
a higher workload at the end of the month when reports
are being processed or the workload
might be really light right before a holiday.
Next, we have throughput.
Throughput is the overall capability of
the database's hardware and software to process requests.
Throughput is made up of the input and output speed,
the central processor unit speed,
how well the machine can run parallel processes,
the database management system,
and the operating system and system software.
Basically, throughput describes
a workload size that the system can handle.
Let's get into resources.
In BI, resources are
the hardware and software tools
available for use in a database system.
This includes the disk space and memory.
Resources are a big part of
a database system's ability to
process requests and handle data.
They can also fluctuate,
especially if the hardware or
other dedicated resources are
shared with additional databases,
software applications, or services.
Also, cloud-based systems are
particularly prone to fluctuation.
It's useful to remember that
external factors can affect performance.
Now we come to optimization.
Optimization involves
maximizing the speed and efficiency with
which data is retrieved in order to
ensure high levels of database performance.
This is one of the most important factors that
BI Professionals return to again and again.
Coming up soon, we're going to
talk about it in more detail.
Finally, the last factor
of database performance is contention.
Contention occurs when two or more components
attempt to use a single resource in a conflicting way.
This can really slow things down.
For instance, if there are
multiple processes trying to
update the same piece of data,
those processes are in contention.
As contention increases,
the throughput of the database decreases.
Limiting contention as much as possible will help
ensure the database is performing at its best.
There you have five factors of database performance,
workload, throughput,
resources, optimization, and contention.
Coming up, we're going to check out
an example of these factors in action
so you can understand more about how
each contributes to database performance. 


## A guide to the five factors of database performance

Database performance is an important consideration for BI professionals. As you have been learning, database performance is a measure of the workload that can be processed by the database, as well as associated costs. Optimization involves maximizing the speed and efficiency that data is retrieved in order to ensure high levels of database performance. This means that your stakeholders have the fastest access to the data they need to make quick and intelligent decisions. You have also been learning that there are five factors of database performance: workload, throughput, resources, optimization, and contention.

The five factors:

_In this reading, you will be given a quick overview of the five factors that you can reference at any time and an example to help outline these concepts. In the example, you are a BI professional working with the sales team to gain insights about customer purchasing habits and monitor the success of current marketing campaigns._

- Workload:
	
The combination of transactions, queries, data warehousing analysis, and system commands being processed by the database system at any given time.
	
On a daily basis, your database needs to process sales reports, perform revenue calculations, and respond to real-time requests from stakeholders.All of these needs represent the workload the database needs to be able to handle.

- Throughput:

The overall capability of the database’s hardware and software to process requests.

The system’s throughput is the combination of input and output speed, the CPU speed, the machine’s ability to run parallel processes, the database management system, and the operating system and system software.

- Resources:

The hardware and software tools available for use in a database system.

The database system is primarily cloud-based, which means it depends on online resources and software to maintain functionality.

- Optimization:

Maximizing the speed and efficiency with which data is retrieved in order to ensure high levels of database performance.

Continually checking that the database is running optimally is part of your job as the team's BI professional.

- Contention:
	
When two or more components attempt to use a single resource in a conflicting way.
	
Because this system automatically generates reports and responds to user-requests, there are times when it may be trying to run the queries on the same datasets at the same time, causing slowdown for users.


## Optimize database performance

Recently, we've been learning
a lot about database performance.
As a refresher, this
is a measure of the workload that can be
processed by the database as well as associated costs.
We also explored optimization,
which is one of the most important factors
of database performance.
You recall that optimization
involves maximizing the speed and
efficiency with which data is retrieved in
order to ensure high levels of database performance.
In this video, we're going to
focus on optimization and how
BI professionals optimized databases by examining
resource use and identifying
better data sources and structures.
Again, the goal is to enable the system to process
the largest possible workload
at the most reasonable cost.
This requires a speedy response time,
which is how long it takes for a database to respond
to a user request. Here's an example.
Imagine you're a BI professional
receiving emails from people on your team
who say that it's taking longer than usual
for them to pull the data they need from the database.
At first, this seems like a pretty minor inconvenience,
but a slow database can be
disruptive and cost your team a lot of time.
If they have to stop and wait whenever they need
to pull data or perform a calculation,
it really affects their work.
There are a few reasons that
users might be encountering this issue.
Maybe the queries aren't fully optimized or
the database isn't properly indexed or partitioned.
Perhaps the data is fragmented,
where there isn't enough memory or CPU.
Let's examine each of these.
First, if the queries users are
writing to interact with the database are inefficient,
it can actually slow down your database resources.
To avoid this, the first step is to simply
revisit the queries to
ensure they're as efficient as possible.
The next step is to consider the query plan.
In a relational database system that uses SQL,
a query plan is a description of the steps
the database system takes in order to execute a query.
As you've learned, a query tells a system what to do,
but not necessarily how to do it.
The query plan is the how.
If queries are running slowly,
checking the query plan to find out if there are steps
causing more draw than necessary can be helpful.
This is another iterative process.
After checking the query plan,
you might rewrite the query or create
new tables and then check the query plan again.
Now let's consider indexing.
An index is an organizational tag
used to quickly locate data within a database system.
If the tables within a database
haven't been fully indexed,
it can take the database longer to locate resources.
In Cloud-based systems working with big data,
you might have data partitions instead of indexes.
Data partitioning is the process
of dividing a database into
distinct logical parts in order to
improve query processing and increase manageability.
The distribution of data within
the system is extremely important.
Ensuring that data has been
partitioned appropriately and consistently,
is part of optimization too.
The next issue is fragmented data.
Fragmented data occurs when data is
broken up into many pieces that are not stored together.
Often as a result of using
the data frequently or creating,
deleting, or modifying files.
For example, if you are accessing the same data
often and versions of it are being saved in your cache,
those versions are actually
causing fragmentation in your system.
Finally, if your database is having
trouble keeping up with your organization's demands,
it might mean there isn't enough memory
available to process everyone's requests.
Making sure your database has the capacity to
handle everything you ask of it it's critical.
Consider our example again.
You received some emails from
the team stating that it was
taking longer than usual to access data from database.
After learning about the slowdown from your team,
you were able to assess
the situation and make some fixes.
Addressing the issues allowed you to ensure
the database was working as
efficiently as possible for your team.
Problem-solved. But database optimization is
an ongoing process and you'll need to
continue to monitor performance
to keep everything running smoothly. 


## Indexes, partitions, and other ways to optimize

- Optimization for data reading

One of the continual tasks of a database is reading data. Reading is the process of interpreting and processing data to make it available and useful to users. As you have been learning, database optimization is key to maximizing the speed and efficiency with which data is retrieved in order to ensure high levels of database performance. Optimizing reading is one of the primary ways you can improve database performance for users. Next, you will learn more about different ways you can optimize your database to read data, including indexing and partitioning, queries, and caching.

- Indexes

Sometimes, when you are reading a book with a lot of information, it will include an index at the back of the book where that information is organized by topic with page numbers listed for each reference. This saves you time if you know what you want to find– instead of flipping through the entire book, you can go straight to the index, which will direct you to the information you need.

Indexes in databases are basically the same– they use the keys from the database tables to very quickly search through specific locations in the database instead of the entire thing. This is why they’re so important for database optimization– when users run a search in a fully indexed database, it can return the information so much faster.  For example, a table with columns ID, Name, and Department could use an index with the corresponding names and IDs.

Now the database can easily locate the names in the larger table quickly for searches using those IDs from the index.

- Partitions

Data partitioning is another way to speed up database retrieval. There are two types of partitioning: vertical and horizontal. Horizontal partitioning is the most common, and involves designing the database so that rows are organized by logical groupings instead of stored in columns. The different rows are stored in different tables– this reduces the index size and makes it easier to write and retrieve data from the database.

Instead of creating an index table to help the database search through the data faster, partitions split larger, unwieldy tables into much more manageable, smaller tables. 

In this example, the larger sales table is broken down into smaller tables– these smaller tables are easier to query because the database doesn’t need to search through as much data at one time.

- Other optimization methods

In addition to making your database easier to search through with indexes and partitions, you can also optimize your actual searches for readability or use your system’s cached memory to save time retrieving frequently used data. 

1. Queries

Queries are requests for data or information from a database. In many cases, you might have a collection of queries that you run regularly; these might be automated queries that generate reports, or regular searches made by users.

If these queries are not optimized, they can take a long time to return results to users and take up database resources in general. There a few things you can do to optimize queries:

    Consider the business requirements: Understanding the business requirements can help you determine what information you really need to pull from the database and avoid putting unnecessary strain on the system by asking for data you don’t actually need.

    Avoid using SELECT* and SELECT DISTINCT: Using SELECT* and SELECT DISTINCT causes the database to have to parse through a lot of unnecessary data. Instead, you can optimize queries by selecting specific fields whenever possible.

    Use INNER JOIN instead of subqueries: Using subqueries causes the database to parse through a large number of results and then filter them, which can take more time than simply JOINing tables in the first place.

Additionally, you can use pre-aggregated queries to increase database read functionality. Basically, pre-aggregating data means assembling the data needed to measure certain metrics in tables so that the data doesn’t need to be re-captured every time you run a query on it.

If you’re interested in learning more about optimizing queries, you can check out Devart’s article on SQL Query Optimization.

2. Caching

Finally, the cache can be a useful way to optimize your database for readability. Essentially, the cache is a layer of short-term memory where tables and queries can be stored. By querying the cache instead of the database system itself, you can actually save on resources. You can just take what you need from the memory.

For example, if you often access the database for annual sales reports, you can save those reports in the cache and pull them directly from memory instead of asking the database to generate them over and over again.

- Key takeaways

This course has focused a lot on database optimization and how you, as a BI professional, can ensure that the systems and solutions you build for your team continue to function as efficiently as possible. Using these methods can be a key way for you to promote database speed and availability as team members access the database system. And coming up, you’re going to have opportunities to work with these concepts yourself!


## Activity: Partition data and create indexes in BigQuery

## Case study: Deloitte - Optimizing outdated database systems

In this part of the course, you have been learning about the importance of database optimization. This basically means maximizing the speed and efficiency with which data is retrieved in order to ensure high levels of database performance. Part of a BI professional’s job is examining resource-use and identifying better data sources and structures. In this case study, you will have an opportunity to explore an example of how the BI team at Deloitte handled optimization when they discovered their current database was difficult for users to query. 

- Company background

Deloitte collaborates with independent firms to provide audit and assurance, consulting, risk and financial advisory, risk management, tax, and related services to select clients. Deloitte’s brand vision is to be a standard of excellence within the field and to uphold their brand values as they develop leading strategies and cutting edge tools for clients to facilitate their business. These values include integrity, providing outstanding value to clients, commitment to community, and strength from cultural diversity. 

- The challenge

Because of the size of the company and their ever-evolving data needs, the database grew and changed to match current problems without time to consider long-term performance. Because of this, the database eventually grew into a collection of unmanaged tables without clear joins or consistent formatting. This made it difficult to query the data and transform it into information that could effectively guide decision making. 

The need for optimization appeared gradually as the team had to continually track data and had to repeatedly test and prove the validity of the data.  With a newly optimized database, the data could more easily be understood, trusted, and used to make effective business decisions.

Primarily, this database contained marketing and financial data that would ideally be used to connect marketing campaigns and sales leads to evaluate which campaigns were successful. But because of the current state of the database, there was no clear way to tie successes back to specific marketing campaigns and evaluate their financial performance. The biggest challenge to this initiative was programming the external data sources to feed data directly into the new database, rather than into the previous tables that were scheduled to be deprecated.  Additionally, the database design needed to account for tables that represented the lifecycle of the data and designed with joins that could easily and logically support different data inquiries and requests.

- The approach

Because of the scale of the project and the specific needs of the organization, the BI team decided to design their own database system that they could implement across the entire organization. That way, the architecture of the database would really capture their data needs and connect tables thoughtfully so they were easier to query and use.

For example, the team wanted to be able to easily connect the initial estimate of a marketing campaign’s financial success with its ending value and how well internal processes were able to predict the success of a campaign. Increases from the initial estimate were good, but if estimates were frequently much higher than actual outcomes, it could indicate an issue with the tooling used to develop those estimates. But in the database’s current state, there were dozens of tables across accounting groups that were creating access issues that were preventing these insights from being made. Also, the different accounting groups had a lot of overlap that the team hoped to more thoughtfully structure for more long-term use.

To achieve these goals, the team strategized the architecture, developed checkpoints to determine if the required functionality could be developed and eventually scaled up, and created an iterative system wherein regular updates to the database system could be made to continue refining it moving forward.

In order to consider the database optimization project a success, the BI team wanted to address the following issues:

    Were the necessary tables and columns consolidated in a more useful way?
    Did the new schema and keys address the needs of analyst teams?
    Which tables were being queried repeatedly and were they accessible and logical?
    What sample queries could promote confidence in the system for users?

A variety of partners and stakeholders had to be involved in the optimization project because so many users across the organization would be affected. The database administrators and engineers working with the BI team were particularly key for this project because they led the design and creation of the database, mapped the life cycle of the data as it matured and changed over time and used that as a framework to construct a logical data-flow design.

These engineers then conducted interviews with various stakeholders to understand the business requirements for teams across the entire organization, trained a team of analysts on the new system, and deprecated the old tables that weren’t working.

- The results

Deloitte’s BI team recognized that, while the database had been continually updated to address evolving business needs, it had grown harder to manage over time. In order to promote greater database performance and ensure their database could meet their needs, the BI team collaborated with database engineers and administrators to design a custom database architecture that thoughtfully addressed the business needs of the organization. For example, the new database structure helped build connections between tables tracking marketing campaigns over time and their successes, including revenue data and regional locations.

This database optimization effort had a lot of benefits. The greatest benefit was the organization’s ability to trust their data–the analyst team didn’t have to spend as much time validating the data before use because the tables were now organized and joined in more logical ways. The new architecture also promoted simpler queries. Instead of having to write hundreds of lines of complicated code to return simple answers, the new database was optimized for simpler, shorter queries that took less time to run.

This provided benefits for teams across the organization:

    The marketing team was able to get better feedback on the value created by specific campaigns.

    The sales team could access specific information about their regions and territories, giving them insights about possible weaknesses and opportunities for expansion.

    The strategy team was able to bridge the gap between the marketing and sales teams, and ultimately create actionable OKRs (Objectives and Key Results) for the future.

However, as you have been learning, database optimization is an iterative process. The BI team’s work didn’t stop once they implemented the new database design. They also designated a team to oversee data governance to ensure the quality of the data and prevent the same problems from happening again. This way, the data remains organized and also this team can continue refining the developed databases based on evolving business needs.

- Conclusion

The databases where your organization stores their data are a key part of the BI processes and tools you create–if the database isn’t performing well, it will affect your entire organization and make it more difficult to provide stakeholders with the data they need to make intelligent business decisions. Optimizing your database promotes high performance and a better user experience for everyone on your team.


## The five factors in action

Earlier, we learned about the five factors of database performance:
Workload, throughput, resources, optimization and contention.
But how do they actually operate within a working system.
Let's explore a database and witness how the five factors affect its performance.
Before we get into how the five factors influence this database,
let's understand how it's been designed.
In this example we'll be checking out a movie theater chain system.
There are a few things that we'll need to consider during optimization.
First let's think about what this database is being used for.
In this case the movie theater chain uses data related to ticket purchases, revenue
and audience preferences in order to make decisions about what movies to play and
potential promotions.
Second we'll consider where the data is coming from.
In this example it's being pushed from multiple
sources into an OLAP system where analysis takes place.
Also the database uses data from individual theaters OLTP systems in order
to explore trends and ticket sales for different movie times and genres.
The OLTP systems that manage transaction data, uses snowflake database model.
At the center there is a fact table capturing the most important
information about the tickets such as whether or
not a specific seat has been reserved, the reservation type, the screening ID.
The employee ID of whoever entered the reservation and the seat number.
In order to capture details about these facts, the model also includes
several dimension tables connected to the fact table with information on employee,
movie, screening, auditorium, seat and reservation.
This database is fairly straightforward and
enables each movie theater to record data in these different tables and
prevents them from accidentally booking the same seat twice.
However, these individual OLTP systems aren't designed for analysis,
which is why the data needs to be pulled into the destination OLAP system.
There, it can be accessed and explored by users in order to gain insights and
make business decisions.
Okay, now that we know a little more about our database,
let's find out how the five factors of database performance influence it.
First as you know, workload is a combination of transactions, queries,
data warehousing analysis and
system commands being processed by the database system at any given time.
In this case, most of the workload is processing user requests such as
generating scheduled reports or fulfilling queries.
If the database can't handle the workload, it might cause the system to crash
disrupting user's ability to access and use the data.
Maybe report requires a lot of resources to generate or
there might be a growing number of analysts accessing this data.
But we know that it's often possible to predict peak workload times.
So we can make adjustments to ensure the system can handle these requests.
Now, let's explore throughput.
Again this is the overall capability of the database's hardware and
software to process requests.
Because our movie theater system is mostly focused on analysis of data from
OLTP databases,
were working with an OLAP database that primarily uses cloud storage.
The database storage processes and the computers within the system,
they're accessing the cloud data.
Need to be capable of handling the theaters workload,
especially when the database system is being used a lot.
The hardware and software that compose the system's throughput are the resources.
For example, the movie theaters might use a cache controller disc to help
the database manage the storage and retrieval of data from the memory systems.
Next we have optimization, which you've already learned a lot about.
Ideally users should be able to access transaction data that has been ingested
from multiple other database systems.
If retrieval slows down, it can take longer to get the data and
provide insights to stakeholders.
This is why keeping the database optimized even after it has been set up is
important.
The last factor, database performance is contention.
The movie theater company has a team with many different analysts accessing and
using this data.
That's in addition to the automated transformations being applied to the data
and the reports being generated.
All these requests can end up competing with each other and cause contention.
And this can potentially be problematic if the system processes multiple
requests at the same time, essentially making the same updates over and over.
To limit this, the database processes queries and
the order the requests are made.
And now, you've gotten a chance to explore how the five factors of database
performance might affect a real database system.
No matter how simple or complex, these are essential considerations for
any BI profession. 


## Determine the most efficient query

So far, you have learned about the factors that affect database performance and database query optimization. This is an important part of a BI professional’s work because it allows them to ensure that the tools and systems their team is using are as efficient as possible. Now that you’re more familiar with these concepts, you’ll review an example. 

- The scenario

Francisco’s Electronics recently launched its home office product line on its e-commerce site. After receiving a positive response from customers, company decision-makers chose to add the rest of their products to the site. Since launch, they have received more than 10,000,000 sales. While this is great for the business, such a massive catalog of sales records has affected the speed of their database. The sales manager, Ed, wanted to run a query for the number of sales created after November 1, 2021, in the “electronics” category but was unable to because the database was too slow. He asked Xavier, a BI analyst, to work with the database and optimize a query to speed up the sales report generation.

To begin, Xavier examined the sales_warehouse database schema shown below. The schema contains different symbols and connectors that represent two important pieces of information: the major tables within the system and the relationships among these tables.

< The sales_warehouse database schema. The Sales table connects to the Products, Users, Locations, and Orders tables. >

The sales_warehouse database schema contains five tables—Sales, Products, Users, Locations, and Orders—which are connected via keys. The tables contain five to eight columns (or attributes) ranging in data type. The data types include varchar or char (or character), integer, decimal, date, text (or string), timestamp, and bit.

The foreign keys in the Sales table link to each of the other tables. The “product_id” foreign key links to the Products table, the “user_id” foreign key links to the Users table, the “order_id” foreign key links to the Orders table, and the “shipping_address_id” and “billing_address_id” foreign keys link to the Locations table.

- Examining the SQL query

After considering the details, Xavier found that the following request needed optimization:

- Optimizing the query

To make this query more efficient, Xavier started by checking if the "date" and "category" fields were indexed. He did this by running the following queries:

Without indexes in the columns used for query restrictions, the engine did a full table scan that processed all several million records and checked which ones had date >= “2021-11-01” and category = “electronics.” 

Then, he indexed the “date” field in the Sales table and the “category” field in the Products table using the following SQL code:

Unfortunately, the query was still slow, even after adding the indices. Assuming that there were only a few thousand sales created after “2021-11-01,” the query still created a very large virtual table (joining Sales and Products). It had millions of records before filtering out sales with a date after “2021-11-01” and sales with products in “electronics” categories. This resulted in an inefficient and slow query.

To make the query faster and more efficient, Xavier modified it to first filter out the sales with dates after “2021-11-01.” The query “(SELECT product_id FROM Sales WHERE date > '2021-11-01') AS oi” returned only a few thousand records, rather than millions of records. He then joined these records with the Products table. 

Xavier’s final optimized query was:

- Key takeaways

Optimizing queries will make your pipeline operations faster and more efficient. In your role as a BI professional, you might work on projects with extremely large datasets. For these projects, it’s important to write SQL queries that are as fast and efficient as possible. Otherwise, your data pipelines might be slow and difficult to work with.



# REVIEW: DYNAMIC DATABASE DESING

## Wrap-up

You've been learning about database design and the role
BI professionals play in creating and
maintaining useful database systems.
So far, you focus on
the five factors of database performance;
workload, throughput,
resources, optimization, and contention.
You also learn some strategies
specifically for database optimization,
and what issues to check for
if your team members start noticing a slowdown.
You even explored how
the five factors can affect actual databases,
database optimization,
and the importance of keeping databases up to speed.
As a BI professional,
developing processes that enable your team to
pull insights themselves is a key part of the job.
But systems and processes change over time,
they stop working or need to be updated.
That's one of the reasons why continuing to
monitor database performance is so important.
The database system should have
lasting high performance levels.
Coming up, you're going to discover more about
optimizing systems and the tools
you'll create as a BI professional.
But first, you have another weekly challenge.
As always, feel free to
check back over any of the material,
and review the glossary to prepare yourself for success.
Once you've completed your assessment,
I'll meet you back here for more about
optimizing ETL processes. Great job. 


## Glossary

Contention: When two or more components attempt to use a single resource in a conflicting way

Data partitioning: The process of dividing a database into distinct, logical parts in order to improve query processing and increase manageability

Database performance: A measure of the workload that can be processed by a database, as well as associated costs

ELT (extract, load, and transform): A type of data pipeline that enables data to be gathered from data lakes, loaded into a unified destination system, and transformed into a useful format 

Fragmented data: Data that is broken up into many pieces that are not stored together, often as a result of using the data frequently or creating, deleting, or modifying files

Index: An organizational tag used to quickly locate data within a database system

Optimization: Maximizing the speed and efficiency with which data is retrieved in order to ensure high levels of database performance

Query plan: A description of the steps a database system takes in order to execute a query

Resources: The hardware and software tools available for use in a database system

Subject-oriented: Associated with specific areas or departments of a business

Throughput: The overall capability of the database’s hardware and software to process requests

Workload: The combination of transactions, queries, data warehousing analysis, and system commands being processed by the database system at any given time
