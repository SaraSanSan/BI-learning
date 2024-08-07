# | The Path to Insights: DATA MODELS & PIPELINES |

# DATA MODELS & PIPELINES

You’ll start this course by exploring data modeling, common schemas, and database elements. You’ll consider how business needs determine the kinds of database systems that BI professionals implement. Then, you’ll discover pipelines and ETL processes, which are tools that move data and ensure that it’s accessible and useful.

Learning Objectives:

    Identify and define key database models and schemas.
    Assess which database design pattern and schema is appropriate for different data.
    Discuss data model alternatives that would be optimal, performant, and adherent to the reporting requirements looking into current data size and growth.
    Define ETL and explain what it means.
    Identify key information from stakeholders necessary to create a data pipeline.
    Describe different types of pipelines.
    Describe the key stages of a data pipeline.
    Understand what a data pipeline is, its objectives, and how it works.


## Course 2 overview

Hello, and welcome to The Path to Insights: Data Models and Pipelines, the second course in the Google Business Intelligence Certificate. You’re on an exciting journey!

By the end of this course, you will be able to use data modeling and ETL processes to extract data from source systems, transform it into formats that better enable analysis, and drive business processes and goals.

### Course descriptions:

The Google Business Intelligence Certificate has three courses. The Path to Insights: Data Models and Pipelines is the second course.

- Foundations of Business Intelligence: Discover the role of BI professionals within an organization and the career paths they typically follow. Then, explore core BI practices and tools and learn how BI professionals use them to make a positive impact on organizations. 

- The Path to Insights: Data Models and Pipelines (current course): Explore data modeling and ETL processes for extracting data from source systems, transforming it into formats that better enable analysis, and driving business processes and goals.

- Decisions, Decisions: Dashboards and Reports: Apply your knowledge of BI and data modeling to create dynamic dashboards that track key performance indicators to meet stakeholder needs.

### Course 2 content

Each course of this certificate program is broken into modules. You can complete courses at your own pace, but the module breakdowns are designed to help you finish the entire Google Business Intelligence Certificate in two to four months. What’s to come? Here’s a quick overview of the skills you’ll learn in each module of this course.

- Module 1: Data models and pipelines

You will start this course by exploring data modeling foundations, as well as common schemas and key database elements. You will also consider how business needs determine the kinds of database systems that a BI professional might implement. You will then shift to learning about pipelines and ETL processes, which are the tools that move data throughout the system and make sure it’s accessible and useful. Along the way, you will add many more important tools to your BI toolbox.

- Module 2: Dynamic database design

In this part of the course, you will learn more about database systems, including data marts, data lakes, data warehouses, and ETL processes. You will also investigate the five factors of database performance: workload, throughput, resources, optimization, and contention. Finally, you will begin thinking about how to design efficient queries that get the most from your system. 

- Module 3: Optimize ETL processes

In this section of the course, you will learn about ETL quality testing, data schema validation, verifying business rules, and general performance testing. You will also explore data integrity and learn how built-in quality checks help you discover data defects. Finally, you will learn how to verify business rules and conduct general performance testing to make sure pipelines fulfill the intended business need. 

- Module 4: Course 2 end-of-course project

In the second end-of-course project, you will create a pipeline process to deliver necessary data to a target table. Then, you will use that target table to develop reports based on project needs. After you create the pipeline, you will also ensure that it is performing correctly and that there are built-in defenses against data quality issues. 


## Introduction to Course 2

As a BI professional,
you aren't just answering your team's questions,
you're empowering them with
the data to answer their own questions.
By pinpointing the answers they require,
you can build tools that enable them to access
and use the data they need when they need it.
Hey, there. Welcome to this course.
If you've already completed the previous one,
you might remember me, but
if you're just joining us, I'm Ed.
I'm a product manager here at Google.
I'm really excited to help you get
started with data models and extract,
transform, and load, or ETL pipelines.
As you've been learning,
BI professionals are responsible for
analyzing data to generate
meaningful insights and solve problems,
answer questions, find patterns,
and inform business decisions.
A large part of this is building tools to
provide stakeholders with ongoing insights.
This course is going to focus on those tools and how to
automate them in order to
pull data from different sources,
monitor it, and provide data-driven insights.
First, you'll learn about
design patterns and database schemas,
including common structures that BI professionals use.
You'll also be introduced to
data pipelines and ETL processes.
You've learned that ETL stands for
extract, transform, and load.
This refers to the process of
gathering data from source systems,
converting it into a useful format,
and bringing it into a data warehouse
or other unified destination system.
This will be an important part of
your job as a BI professional.
You'll also develop strategies
for gathering information from stakeholders
in order to help you develop
more useful tools and processes for your team.
After that, you'll focus
on database optimization to reduce
response time or the time it takes
for a database to complete a user request.
This will include exploring different types of
databases and the five factors of database performance,
workload, throughput,
resources, optimization, and contention.
Finally, you'll learn about the importance
of quality testing your ETL processes,
validating your database schema,
and verifying business rules.
Once you've finished this course,
you'll apply your skills to
a realistic business scenario,
which is a great way to demonstrate
your BI knowledge to potential employers.
As you've been learning, a large part of BI is
making other people's jobs easier by automating,
simplifying, and enhancing their processes.
For example, in one of my projects I helped the
central finance team
aggregate years' worth of global sales.
This allowed my team to identify
the underlying drivers that affected
trends in prices and quantities sold.
They were then able to clearly report
these findings to key stakeholders.
I love solving problems and making
my teams lives a little easier which is
one of the reasons why I'm so excited to teach you more
about data modeling and pipelines in this course.
All right, let's get started. 


## Ed: Overcome imposter syndrome

Hi. I'm Ed.
I'm a Product Manager at Google.
As a product manager,
I define the vision for a product
and make sure that it aligns with what users
actually need that product to do for them.
For me, imposter syndrome is a belief
that you are not where you need to be,
in terms of your skill,
your perspectives, background, or your experience.
I've definitely experienced imposter syndrome.
I work with a lot of people
who are very skilled in their areas of expertise.
Not everyone can have every
single skill across the board.
You end up thinking,
oh, maybe I should be able to program like her,
or maybe I should be as good a data scientist as him,
and maybe I should have this level of perspective
as it seems like everyone around me does as well.
That's not necessarily true.
I really think it's important to focus on
the unique perspective that you provide,
because everyone's perspective
and expertise and interest,
and the way in which they're going to apply all of those,
they're all going to differ.
There are unique combinations of things
that you provide that other people cannot provide,
simply by virtue of the fact that you are you.
I found that the most useful technique in overcoming
Imposter syndrome is being vulnerable
and transparent that you feel that way.
Find people that you trust,
find people that you can speak with
and tell them how you're feeling.
Tell them why you're feeling that way.
Feeling a certain way doesn't have to be
an indication of who you are or what you're capable of.
It simply is.
Being able to be vulnerable and say, hey,
I don't understand this,
or I would like a little bit extra information,
that can be helpful,
not only for you, but also for people around you.
We tend to focus on the negatives.
We tend to focus on the challenges or
the constructive aspects that
we might see that we need to improve on.
While not giving ourselves enough credit
for the things that we do well,
the things that are strengths
that we should lean more into.
You're going to be more successful
by understanding and really leaning into
your strengths than simply trying
to hide or runaway from your failures. 



# GET STARTED WITH DATA MODELING, SCHEMAS & DATABASES

## Welcome to module 1

Welcome to the first section of this course. You're going to learn about how BI
professionals use data models to help them build database systems,
how schemas help professionals understand and organize those systems and
how pipeline processes move data from one part of the system to another.
We'll start by exploring data modeling foundations as well as common schemas and
key database elements. We'll also consider how business needs determine the kinds of
database systems that a BI professional might implement.
We'll then shift to pipelines and ETL processes, which are the tools that move
data throughout the system and make sure it's accessible and useful.
By the time you're done, you'll have added many more important tools to your BI
toolbox. Let's get started. 


## Data modeling, design patterns, and schemas

In this video, we're going to explore data modeling,
design patterns, and schemas.
If you've been working with databases or if
you're coming from the Google Data Analytics certificate,
you may be familiar with
data modeling as a way to think about organizing data.
Maybe you're even already using
schemas to understand how databases are designed.
As you've learned, a database is
a collection of data stored in a computer system.
In order to make databases useful,
the data has to be organized.
This includes both source systems
from which data is ingested and
moved and the destination
database where it will be acted upon.
These source systems could include data lakes,
which are database systems that store large amounts of
raw data in its original format until it's needed.
Another type of source system is
an Online Transaction Processing or OLTP database.
An OLTP database is one that has been
optimized for data processing instead of analysis.
One type of destination system is a data mart,
which is a subject oriented database that
can be a subset of a larger data warehouse.
Another possibility is using
an Online Analytical Processing or OLAP database.
This is a tool that has been
optimized for analysis in addition to
processing and can analyze data from multiple databases.
You will learn more about these things later.
But for now, just understand that a big part of
a BI professional's responsibility
is to create the destination database model.
Then it will organize the systems,
tools and storage accordingly,
including designing how the data is organized and stored.
These systems all play a part in
the tools you'll be building later on.
They're important foundations for key BI processes.
When it comes to organization,
you likely know that there are two types of
data: unstructured and structured.
Unstructured data is not organized
in any easily identifiable manner.
Structure data has been organized in a certain format,
such as rows and columns.
If you'd like to revisit different data types,
take a moment to review
this information from the Data Analytics certificate.
Now, it can be tricky to understand structure.
This is where data modeling comes in.
As you learned previously,
a data model is a tool for organizing
data elements and how they relate to one another.
These are conceptual models that help
keep data consistent across the system.
This means that give us an idea of
how the data is organized in theory.
Think back to Furnese's
perfect train of business intelligence.
A data model is like a map of that train system.
It helps you navigate the database by
giving you directions through the system.
Data modeling is a process of creating these tools.
In order to create the data model,
BI professionals will often use
what is referred to as a design pattern.
Design pattern is a solution that uses relevant measures
and facts to create a model to support business needs.
Think of it like a re-usable problem-solving template,
which may be applied to many different scenarios.
You may be more familiar with the output of
the design pattern, a database schema.
As a refresher, a schema is a way of
describing how something such as data is organized.
You may have encountered schemas
before while working with databases.
For example, some common schemas you
might be familiar with include relational models,
star schemas, snowflake schemas and noSQL schemas.
These different schemas enabled us to
describe the model being used to organize the data.
If the design pattern is the template for
the data model then
the schema is the summary of that model.
Because BI professionals play
such an important role in creating these systems,
understanding data modeling is
an essential part of the job.
Coming up, you're going to learn
more about how design patterns and schemas
are used in BI and get a chance to practice
data modeling yourself. Bye for now. 


## Get the facts with dimensional models

If you've been working with database SQL
you're probably already familiar with relational databases. In this video,
you're going to return to the concept of relational databases and
learn about a specific kind of relational modeling technique that is used in
business intelligence: dimensional modeling. As a refresher,
a relational database contains a series of tables that can
be connected to form relationships.
These relationships are established using primary and foreign keys.
Check out this car dealership database. Branch ID
is the primary key in the car dealerships table, but
it is the foreign key in the product details table.
This connects these two tables directly.
VIN is the primary key in the product details table and
the foreign key in the repair parts table.
Notice how these connections actually create relationships between all
of these tables.
Even the car dealerships and
repair parts tables are connected by the product details table.
If you took the Google Data Analytics Certificate,
you learn that a primary key is an identifier in the database that references
a column in which each value is unique.
For BI, we're going to expand this idea.
A primary key is an identifier in a database that references a column or
a group of columns in which each row uniquely identifies each record in the table.
In this database we have primary keys in each table.
Branch ID, VIN, and part ID.
A foreign key is a field within a database table that's a primary key in
another table.
The primary keys from each table also appear as foreign keys in other tables.
Which builds those connections.
Basically, a primary key can be used to impose constraints on the database that ensure
data in a specific column is unique by specifically identifying a record
in a relational database table. Only one primary key can exist in a table,
but a table may have many foreign keys.
Okay now let's move on to dimensional models.
A dimensional model is a type of relational model that has been optimized
to quickly retrieve data from a data warehouse.
Dimensional models can be broken down into facts for measurement and
dimensions that add attributes for context. In a dimensional model,
a fact is a measurement or metric.
For example a monthly sales number could be a fact and a dimension is a piece of
information that provides more detail and context regarding that fact.
It's the who, what, where, when, why and how.
So if our monthly sales number is the fact then the dimensions could be
information about each sale, including the customer, the store location and
what products were sold. Next, let's consider attributes.
If you earned your Google Data Analytics certificate,
you learned about attributes in tables.
An attribute is a characteristic or quality of data
used to label the table columns. In dimensional models,
attributes work kind of the same way. An attribute is a characteristic or quality
that can be used to describe a dimension.
So a dimension provides information about a fact and
an attribute provides information about a dimension.
Think about a passport.
One dimension on your passport is your hair and eye color.
If you have brown hair and eyes,
brown is the attribute that describes that dimension.
Let's use another simple example to clarify this; in our car dealership
example if we explore the customer dimension we might have attributes
such as name, address and phone number listed for each customer.
Now that we've established the facts, dimensions, and attributes,
It's time for the dimensional model to use these
things to create two types of tables: fact tables and dimension tables.
A fact table contains measurements or metrics related to a particular event.
This is the primary table that contains the facts and
their relationship with the dimensions.
Basically each row in the fact table represents one event.
The entire table could aggregate several events such as sales in a day.
A dimension table is where attributes of the dimensions of a fact are stored.
These tables are joined the appropriate fact table using the foreign key.
This gives meaning and context to the facts.
That's how tables are connected in the dimensional model.
Understanding how dimensional modeling builds connections will help you
understand database design as a BI professional.
This will also clarify database schemas which are the output of design patterns.
Coming up, we're going to check out different kinds of schemas that result from this type of
modeling to understand how these concepts work in practice !


## Dimensional models with star and snowflake schemas

In a previous video, we explored how BI professionals used dimensional models.
They make it possible to organize data using connected facts, dimensions and
attributes, to create a design pattern.
A schema is the final output of that pattern.
As you've learned, a schema is a way of describing how something, such as data, is organized.
In a database,
it's the logical definition of the data elements, physical characteristics, and
inter-relationships that exist within the model.
Think of the schema like a blueprint, it doesn't hold data itself, but
describes the shape of the data and how it might relate to other tables or models.
Any entry in the database is an instance of that schema and
will contain all of the properties described in the schema.
There are several common schemas that you may encounter in business intelligence,
including star, snowflake and denormalized, or NoSQL schemas.
Star and snowflake schemas are some of the most common iterations of an actual
dimensional model in practice.
A star schema is a schema consisting of one fact table that references any
number of dimension tables.
As its name suggests, this schema is shaped like a star.
Notice how each of the dimension tables is connected to the fact table at the center.
Star schemas are designed to monitor data instead of analyzing it.
In this way, they enable analysts to rapidly process data.
Therefore they're ideal for high scale information delivery, and
they make output more efficient because of the limited number of tables and
clear direct relationships.
Next we have snowflake schemas, which tend to be more complicated than star schemas,
but the principle is the same.
A snowflake schema is an extension of a star schema with additional dimensions
and, often, subdimensions.
These dimensions and subdimensions break down the schema into even more specific
tables, creating a snowflake pattern.
Like snowflakes in nature, a snowflake schema and
the relationships within it can be complex.
Here's an example, notice how the fact table is still at the center,
but now there are subdimension tables connected to the dimension tables,
which gives us a more complicated web.
Now you have a basic idea of the common schemas you might encounter in BI.
Understanding schemas can help you recognize the different ways databases
are constructed and how BI professionals influence database functionality.
Later on, you're going to have more opportunities to explore these different
schemas and even construct some yourself. 


## Design efficient database systems with schemas

You have been learning about how business intelligence professionals use data models and schemas to organize and optimize databases. As a refresher, a schema is a way of describing the way something is organized. Think about data schemas like blueprints of how a database is constructed. This is very useful when exploring a new dataset or designing a relational database. A database schema represents any kind of structure that is defined around the data. At the most basic level, it indicates which tables or relations make up the database, as well as the fields included on each table.

This reading will explain common schema types you might encounter on the job.

### Types of schemas

- Star and snowflake

You’ve already learned about the relational models of star and snowflake schemas. Star and snowflake schemas share some things in common, but they also have a few differences. For instance, although they both share dimension tables, in snowflake schemas, the dimension tables are normalized. This splits data into additional tables, which makes the schemas a bit more complex.

A STAR schema is a schema consisting of one or more fact tables referencing any number of dimension tables. As its name suggests, this schema is shaped like a star. This type of schema is ideal for high-scale information delivery and makes read output more efficient. It also classifies attributes into facts and descriptive dimension attributes (product ID, customer name, sale date).

Here’s an example of a star schema:

In this example, this company uses a star schema to keep track of sales information within their tables. This includes:

    Customer information
    Product information
    The time the sale is made
    Employee information

All the dimension tables link back to the sales_fact table at the center, which confirms this is a star schema.

A SNOWFLAKE schema is an extension of a star schema with additional dimensions and, often, subdimensions. These dimensions and subdimensions create a snowflake pattern. Like snowflakes in nature, a snowflake schema—and the relationships within it—can be complex. Snowflake schemas are an organization type designed for lightning-fast data processing.

Below is an example of a snowflake schema:

Perhaps a data professional wants to design a snowflake schema that contains sports player/club information. Start at the center with the fact table, which contains:

    PLAYER_ID
    LEAGUE_ID
    MATCH_TYPE
    CLUB_ID

This fact table branches out to multiple dimension tables and even subdimensions. The dimension tables break out multiple details, such as player international and player club stats, transfer history, and more.

- Flat model

Flattened schemas are extremely simple database systems with a single table in which each record is represented by a single row of data. The rows are separated by a delimiter, like a column, to indicate the separations between records. Flat models are not relational; they can’t capture relationships between tables or data items. Because of this, flat models are more often used as a potential source within a data system to capture less complex data that doesn’t need to be updated.

Here is a flat table of runners and times for a 100-meter race:

This data isn’t going to change because the race has already occurred. And, it’s so simple, it’s not really worth the effort of integrating it into a complex relational database when a simple flat model suffices.

As a BI professional, you may encounter flat models in data sources that you want to integrate into your own systems. Recognizing that these aren’t already relational models is useful when considering how best to incorporate the data into your target tables.

- Semi-structured schemas

In addition to traditional, relational schemas, there are also semi-structured database schemas which have much more flexible rules, but still maintain some organization. Because these databases have less rigid organizational rules, they are extremely flexible and are designed to quickly access data.

There are four common semi-structured schemas:

> Document schemas store data as documents, similar to JSON files. These documents store pairs of fields and values of different data types.

> Key-value schemas pair a string with some relationship to the data, like a filename or a URL, which is then used as a key. This key is connected to the data, which is stored in a single collection. Users directly request data by using the key to retrieve it.

> Wide-column schemas use flexible, scalable tables. Each row contains a key and related columns stored in a wide format.

> Graph schemas  store data items in collections called nodes. These nodes are connected by edges, which store information about how the nodes are related. However, unlike relational databases, these relationships change as new data is introduced into the nodes.

- Conclusion:

As a BI professional, you will often work with data that has been organized and stored in different ways. Different database models and schemas are useful for different things, and knowing that will help you design an efficient database system!


## Different data types, different databases

As we continue our discussion of data based modeling and schemas,
it's important to understand that there are different facets of databases
that a business intelligence professional might need to consider for
their organization.
This is because the database framework, including how platforms are organized and
how data is stored and processed, affects how data is used.
Let's start with an example. Think about a grocery stores database systems.
They manage daily business processes and analyze and draw insights from data.
For example, in addition to enabling users to manage sales, a grocer's database must
help decision makers understand what items customers are buying and
which promotions are the most effective.
In this video, we're going to check out a few examples of database frameworks and
learn how they're different from one another.
In particular, databases vary based on how the data is processed,
organized and stored.
For this reason it's important to know what type of database your company
is using.
You will design different data models depending on how data is stored and
accessed on that platform.
In addition, another key responsibility for
BI professionals is to facilitate database migrations,
which are often necessary when technology changes and businesses grow.
A database migration involves moving data from one source platform to another target
database.
During a migration users transition the current database schemas,
to a new desired state.
This could involve adding tables or columns, splitting fields,
removing elements, changing data types or other improvements.
The database migration process often requires numerous phases and iterations,
as well as lots of testing.
These are huge projects for BI teams and you don't necessarily just want to take
the original schema and use it in the new one.
So in this video we'll discuss several types of databases including OLTP,
OLAP, Row-based, columnar, distributed, single-homed,
separated storage and compute and combined databases.
The first two database technologies were going to explore, OLTP and
OLAP systems, are based on how data is processed.
As you've learned, an online transaction processing or OLTP database is one
that has been optimized for data processing instead of analysis. 


## Database comparison checklist

In this lesson, you have been learning about the different aspects of databases and how they influence the way a business intelligence system functions. The database framework—including how platforms are organized and how data is stored and processed—affects how data is used. Therefore, understanding different technologies helps you make more informed decisions about the BI tools and processes you create. This reading provides a breakdown of databases including OLAP, OLTP, row-based, columnar, distributed, single-homed, separated storage and compute, and combined.

### OLAP versus OLTP

Database technology  /  Description  /  Use

- OLAP
    · Online Analytical Processing (OLAP) systems are databases that have been primarily optimized for analysis.
	
        Provide user access to data from a variety of source systems
        Used by BI and other data professionals to support decision-making processes
        Analyze data from multiple databases
        Draw actionable insights from data delivered to reporting tables

- OLTP
	· Online Transaction Processing (OLTP) systems are databases that have been optimized for data processing instead of analysis.
	
        Store transaction data
        Used by customer-facing employees or customer self-service applications
        Read, write, and update single rows of data
        Act as source systems that data pipelines can be pulled from for analysis


### Row-based versus columnar

Database technology  /  Description  /  Use

- Row-based
	· Row-based databases are organized by rows.
	
        Traditional, easy to write database organization typically used in OLTP systems
        Writes data very quickly
        Stores all of a row’s values together
        Easily optimized with indexing

- Columnar
	· Columnar databases are organized by columns instead of rows.
	
        Newer form of database organization, typically used to support OLAP systems
        Read data more quickly and only pull the necessary data for analysis
        Stores multiple row’s columns together


### Distributed versus single-homed

Database technology  /  Description  /  Use

- Distributed
	· Distributed databases are collections of data systems distributed across multiple physical locations.
	
        Easily expanded to address increasing or larger scale business needs
        Accessed from different networks
        Easier to secure than a single-homed database system

- Single-homed
	· Single-homed databases are databases where all of the data is stored in the same physical location.
	
        Data stored in a single location is easier to access and coordinate cross-team
        Cuts down on data redundancy
        Cheaper to maintain than larger, more complex systems


### Separated storage and compute versus combined

Database technology  /  Description  /  Use

- Separated storage and compute
	· Separated storage and computing systems are databases where less relevant data is stored remotely, and relevant data is stored locally for analysis.
	
        Run analytical queries more efficiently because the system only needs to process the most relevant data
        Scale computation resources and storage systems separately based on your organization’s custom needs

- Combined storage and compute
	· Combined systems are database systems that store and analyze data in the same place.
	
        Traditional setup that allows users to access all possible data at once
        Storage and computation resources are linked, so resource management is straightforward



# CHOOSE THE RIGHT DATABASE

## The shape of the data

You've been investigating data modeling and
database schemas as well as how different types of databases are used in BI.
Now we're going to explore how these concepts can be used to design data
warehouses.
But before we get into data warehouse design,
let's get a refresher on what a data warehouse actually is.
As you probably remember from earlier in this course,
a database is a collection of data stored in a computer system.
Well, a data warehouse is a specific type of database
that consolidates data from multiple source systems for
data consistency, accuracy and efficient access.
Data warehouses are used to support data driven decision making.
Often these systems are managed by data warehousing specialists but
BI professionals may help design them when it comes to designing a data warehouse.
There are a few important things that BI professional will consider.
Business needs, the shape and volume of the data and
what model the data warehouse will follow.
Business needs are the questions the organization wants to answer or
the problems they want to solve.
These needs help determine how it will use store and organize its data.
For example, hospital storing patient records to monitor health changes
has different data requirements than a financial firm analyzing market trends to
determine investment strategies.
Next let's explore the shape and volume of data from the source system.
Typically the shape of data refers to the rows and
columns of tables within the warehouse and how they are laid out.
The volume of data currently and in the future also changes how the warehouse is
designed and the model the warehouse will follow includes all of the tools and
constraints of the system, such as the database itself and
any analysis tools that will be incorporated into the system.
Let's return to our bookstore example to develop its data warehouse.
We first need to work with stakeholders to determine their business needs.
You'll have an opportunity to learn more about gathering information from
stakeholders later.
But for now let's say they tell us that they're interested in
measuring store profitability and
website traffic in order to evaluate the effectiveness of annual promotions.
Now we can look at the shape of the data.
Consider the business processes or events that are being captured by tables
in the system because this is a retail store.
The primary business process is sales.
We could have a sales table that includes information such as quantity ordered,
total based amount, total tax amount, total discounts and total net amount.
These are the facts as a refresher.
A fact is a measurement or metric used in the business process.
These facts could be related to a series of dimension tables that provide more
context.
For instance, store, customer product promotion,
time, stock or currency could all be dimensions.
The information in these tables gives more context to our fact tables which record
the business processes and events.
Notice how this data model is starting to shape up.
There are several dimension tables all connected to a fact table at the center
and this means we just created a star schema.
With this model, you can answer the specific question,
the effectiveness of annual promotions and
also generate a dashboard with other KPIs and drill down reports.
In this case, we started with the businesses specific needs,
looked at the data dimensions we had and
organize them into tables that formed relationships.
Those relationships helped us determine that a star schema will be the most useful
way to organize this data warehouse.
Understanding the logic behind data warehouse design will help
you develop effective by processes and systems coming up,
you're going to work more with database schemas and
learn about how data is pulled into the warehouse from other sources. 


## Design useful database schemas

Earlier, we learned about what
considerations go into designing data warehouses.
Based on the business needs and the
shape of the data in our previous example,
we created the dimensional model with a star schema.
That process is sometimes called Logical data modeling.
This involves representing different tables
in the physical data model.
Decisions have to be made about
how a system will implement that model.
In this video, we're going to learn more about
what a schema needs to have for it to be functional.
Later, you will use your database schema to validate
incoming data to prevent
system errors and ensure that the data is useful.
For all of these reasons,
it's important to consider the schema
early on in any BI project.
There are four elements a database schema should include.
The relevant data, names
and data types for each column and each table.
Consistent formatting across data entries
and unique keys for every database entry and object.
As we've already learned,
a database schema is a way of
describing how data is organized.
It doesn't actually contain the data itself,
but describes how the data is
shaped and the relationships within the database.
It needs to include all of the data being described.
Or else it won't be a very useful guide for
users trying to understand how the data is laid out.
Let's return to our bookstore database example.
We know that our data contains
a lot of information about the promotions,
customers, products, dates, and sales.
If our schema doesn't represent that,
then we're missing key information.
For instance, it's often
necessary for a BI professional to add
new information to an existing schema if
the current schema can't
answer a specific business question.
If the business wants to know
which customer service employee
responded the most to requests,
we would need to add that information to
the data warehouse and update the schema accordingly.
The schema also needs to include names and
data types for each column
in each table within the database.
Imagine if you didn't organize your kitchen drawers,
it would be really difficult to find anything if
all of your utensils were just thrown together.
Instead, you probably have
a specific place where you keep
your spoons, forks and knives.
Columns are like your kitchen drawer organizers.
They enable you to know what items go
where in order to keep things functioning.
Your schema needs to include the column names
and the data type to indicate what data belongs there.
In addition to making sure the schema
includes all of the relevant data,
names and data types for each column,
it's also important to have consistent formatting
across all of the data entries in the database.
Every data entry is an instance of the schema.
For example, imagine we have
two transactional systems that
we're combining into one database.
One tracks the promotion sent to users,
and the other tracks sales to customers.
In the source systems,
the marketing system that tracks
promotions could have a user ID column,
while the sale system has customer ID instead.
To be consistent in our warehouse schema,
we'll want to use just one of these columns.
In the schema for this database,
we might have a column in one of
our tables for product prices.
If this data is stored
as string type data instead of numerical data,
it can't be used in calculations
such as adding sales together in a query.
Additionally, if any of the data entries
have columns that are empty or missing values,
this might cause issues.
Finally, it's important that there are
unique keys for each entry within the database.
We covered primary and foreign keys in previous videos.
These are what build
connections between tables and enable
us to combine relevant data from
cross the entire database.
In summary, in order for a database schema to be useful,
it should contain the relevant data from the database,
the names and data types for each column and each table,
consistent formatting across all of the entries within
the database and unique keys connecting the tables.
These four elements will ensure that
your schema continues to be useful.
Developing your schema is an ongoing process.
As your data or business needs change,
you can continue to adapt
the database schema to address these needs.
More to come on that soon. 


## Four key elements of database schemas

Whether you are creating a new database model or exploring a system in place already, it is important to ensure that all elements exist in the schema. The database schema enables you to validate incoming data being delivered to your destination database to prevent errors and ensure the data is immediately useful to users.

Here is a checklist of common elements a database schema should include:

- The relevant data: The schema describes how the data is modeled and shaped within the database and must encompass all of the data being described.

- Names and data types for each column: Include names and data types for each column in each table within the database.

- Consistent formatting: Ensure consistent formatting across all data entries. Every entry is an instance of the schema, so it needs to be consistent.

- Unique keys: The schema must use unique keys for each entry within the database. These keys build connections between the tables and enable users to combine relevant data from across the entire database.

Key takeaways:

As you receive more data or business needs change, databases and schemas may also need to change. Database optimization is an iterative process, which means you may need to check the schema multiple times throughout the database’s useful life. Use this checklist to help you ensure that your database schema remains functional.


## Review a database schema

So far, you’ve learned about the differences between various types of database schemas, the factors that influence the choice of database schemas, and how to design a database schema for a data warehouse using best practices.

In this reading, you’ll review a database schema created for a fictional scenario and explore the reasoning behind its design. In your role as a BI professional, you’ll need to understand why a database was built in a certain way. 

- Database schema 

Francisco’s Electronics is launching an e-commerce store for its new home office product line. If it’s a success, company decision-makers plan to bring the rest of their products online as well. The company brought on Mia, a senior BI engineer, to help design its data warehouse. The database needed to store order data for analytics and reporting, and the sales manager needed to generate reports quickly to track the sales so that the success of the site can be determined.

Below is a diagram of the schema of the sales_warehouse database Mia designed. It contains different symbols and connectors that represent two important pieces of information: the major tables within the system and the relationships among these tables.

< The sales_warehouse database schema. The Sales table connects to the Products, Users, Locations, and Orders tables. >

The sales_warehouse database schema contains five tables: Sales, Products, Users, Locations, and Orders, which are connected via keys. The tables contain five to eight columns (or attributes) that range in data type. The data types include varchar or char (or character), integer, decimal, date, text (or string), timestamp, bit, and other types depending on the database system chosen.

- Review the database schema:

To understand a database schema, it’s helpful to understand the purpose of using certain data types and the relationships between fields. The answers to the following questions justify why Mia designed Francisco’s Electronics’ schema this way:

- What kind of database schema is this? Why was this type of database selected? 

Mia designed the database with a star schema because Francisco’s Electronics is using this database for reporting and analytics. The benefits of star schema include simpler queries, simplified business reporting logic, query performance gains, and fast aggregations. 

- What naming conventions are used for the tables and fields? Are there any benefits of using these naming conventions? 

This schema uses a snake case naming convention. In snake case, underscores replace spaces and the first letter of each word is lowercase. Using a naming convention helps maintain consistency and improves database readability. Since snake case for tables and fields is an industry standard, Mia used it in the database.

- What is the purpose of using the decimal fields in data elements? 

For fields related to money, there are potential errors when calculating prices, taxes, and fees. You might have values that are technically impossible, such as a value of  $0.001, when the smallest value for the United States dollar is one cent, or $0.01. To keep values consistent and avoid accumulated errors, Mia used a decimal(10,2) data type, which only keeps the last two digits after the decimal point. 
Note: Other numeric values, such as exchange rate and quantities, may need extra decimal places to minimize rounding differences in calculations. Also, other data types may be better suited for other fields. To track when an order is created (created_at), you can use a timestamp data type. For other fields with various text sizes, you can use varchar. 

- What is the purpose of each foreign and primary key in the database?

Mia designed the Sales table with a primary key ID and included foreign keys in the other tables to reference the primary keys. The foreign keys must be the same data type as their corresponding primary keys. As you’ve learned, primary keys uniquely identify precisely one record on a table, and foreign keys establish integrity references from that primary key to records in other tables.

Sales table key id & foreign keys  /  Associated table

    order_id                           Orders table
    product_id                         Products table
    user_id                            Users table
    shipping_address_id                Locations table
    billing_address_id                 Locations table

- Key takeaways:

In this reading, you explored why a database schema was designed in a certain way. In the world of business intelligence, you’ll spend a lot of time modeling business operations with data, exploring data, and designing databases. You can apply your knowledge of this database schema’s design to build your own databases in the future. This will enable you to use and store data more efficiently in your career as a BI professional.



# HOW DATA MOVES

## Data pipelines and the ETL process

So far, we've been learning a lot
about how data is organized and stored
within data warehouses and how
schemas described those systems.
Part of your job as a BI professional
is to build and maintain a data warehouse,
taking into consideration all of these systems
that exist and are collecting and creating data points.
To help smooth this process,
we use data pipelines.
As a refresher, a data pipeline
is a series of processes that transports
data from different sources to
their final destination for storage and analysis.
This automates the flow of data from sources to targets
while transforming the data to make it
useful as soon as it reaches its destination.
In other words, data pipelines are
used to get data from point A to point B,
automatically save time and
resources and make data more accessible and useful.
Basically, data pipelines to find what,
where, and how data is combined.
They automate the processes
involved in extracting, transforming,
combining, validating,
and loading data for further analysis and visualization.
Effective data pipelines also help
eliminate errors and combat system latency.
Having to manually move data
over and over whenever someone asks for
it or to update a report
repeatedly would be very time-consuming.
For example, if a weather station is
getting daily information about weather conditions,
it will be difficult to manage it
manually because of the sheer volume.
They need a system that takes
in the data and gets it where it
needs to go so it can be transformed into insights.
One of the most useful things about
a data pipeline is that it can
pull data from multiple sources,
consolidate it, and then
migrate it over to its proper destination.
These sources can include relational databases,
a website application with
transactional data or an external data source.
Usually, the pipeline has
a push mechanism that enables it to ingest
data from multiple sources in near
real time or regular intervals.
Once the data has been pulled into the pipeline,
it can be loaded to its destination.
This could be a data warehouse,
data lake or data mart,
which we'll learn more about coming up.
Or it can be pulled directly into a BI
or analytics application for immediate analysis.
Often while data is being moved from point A to point B,
the pipeline is also transforming the data.
Transformations include sorting, validation,
and verification, making the data easier to analyze.
This process is called the ETL system.
ETL stands for extract, transform, and load.
This is a type of data pipeline that
enables data to be gathered from source systems,
converted into a useful format,
and brought into a data warehouse
or other unified destination system.
ETL is becoming more and
more standard for data pipelines.
We're going to learn more about it later on.
Let's say a business analyst has data in
one place and needs to move it to another,
that's where a data pipeline comes in.
But a lot of the time,
the structure of the source system isn't
ideal for analysis which is why
a BI professional wants to transform
that data before it gets to the destination system
and why having set database schemas
already designed and ready to
receive data is so important.
Let's now explore these steps in a little more detail.
We can think of a data pipeline
functioning in three stages,
ingesting the raw data,
processing and consolidating it into categories,
and dumping the data into
reporting tables that users can access.
These reporting tables are referred to as target tables.
Target tables are the predetermined locations where
a pipeline data is sent in order to be acted on.
Processing and transforming data
while it's being moved is
important because it ensures
the data is ready to be used when it arrives.
But let's explore this process in action.
Say we're working with an online streaming service
to create a data pipeline.
First, we'll want to
consider the end goal of our pipeline.
In this example, our stakeholders want to understand
their viewers demographics to inform marketing campaigns.
This includes information about
their viewers ages and interests,
as well as where they are located.
Once we've determined what the stakeholders goal is,
we can start thinking about what data
we need the pipeline to ingest.
In this case, we're going to
want demographic data about the customers.
Our stakeholders are interested in monthly reports.
We can set up our pipeline to automatically
pull in the data we want at monthly intervals.
Once the data is ingested,
we also want our pipeline to
perform some transformations,
so that it's clean and consistent
once it gets delivered to our target tables.
Note that these tables would have already
been set up within our database to receive the data.
Now, we have our customer demographic data and
their monthly streaming habits in
one table ready for us to work with.
The great thing about data pipelines
is that once they're built,
they can be scheduled to automatically
perform tasks on a regular basis.
This means BI team members can
focus on drawing business insights from
the data rather than having to
repeat this process over and over again.
As a BI professional,
a big part of your job will
involve creating these systems,
ensuring that they're running correctly,
and updating them whenever business needs change.
The valuable benefit that
your team will really appreciate. 


## Maximize data through the ETL process

We've been learning a lot about
data pipelines and how they work.
Now, we're going to discuss
a specific kind of pipeline: ETL.
I mentioned previously that ETL
enables data to be gathered from source systems,
converted into a useful format,
and brought into a data warehouse or
other unified destination system.
Like other pipelines, ETL processes work in
stages and these stages are extract, transform, and load.
Let's start with extraction.
In this stage, the pipeline accesses
a source systems and then read and
collects the necessary data from within them.
Many organizations store
their data in transactional databases,
such as OLTP systems,
which are great for logging records
or maybe the business uses flat files,
for instance, HTML or log files.
Either way, ETL makes the data useful for analysis by
extracting it from its source and
moving it into a temporary staging table.
Next we have transformation.
The specific transformation activities
depend on the structure and
format of the destination
and the requirement of the business case,
but as you've learned,
these transformations generally include validating,
cleaning, and preparing the data for analysis.
This stage is also when
the ETL pipeline maps the datatypes from
the sources to the target systems so
the data fits the destination conventions.
Finally, we have the loading stage.
This is when data is delivered to its target destination.
That could be a data warehouse, a data lake,
or an analytics platform that
works with direct data feeds.
Note that once the data has been delivered,
it can exist within multiple locations
in multiple formats.
For example, there could be
a snapshot table that covers a week of
data and a larger archive
that has some of the same records.
This helps ensure the historical data
is maintained within
the system while giving stakeholders
focused, timely data,
and if the business is interested in
understanding and comparing average monthly sales,
the data would be moved to
an OLAP system that have
been optimized for analysis queries.
ETL processes are a common type of
data pipeline that BI professionals
often build and interact with.
Coming up, you're going to learn
more about these systems and how they're created. 


## Choose the right tool for the job 

In previous videos, we've been exploring pipeline processes that ingest 
data from different sources, transform it to match the destination formatting,
and push it to a final destination where users can start drawing business insights.
BI professionals play a key role in building and maintaining these processes,
and they use a variety of tools to help them get the job done.
In this video, we'll learn how BI professionals choose the right tool.
As a BI professional, your organization will likely have preferred vendors,
which means you'll be given a set of available BI solutions.
One of the great things about BI is that different tools have very similar
principles behind them and similar utility.
This is another example of a transferable skill.
In other words, your general understanding can be applied to other solutions,
no matter which ones your organization prefers.
For instance,
the first database management system I learned was Microsoft Access.
This experience helped me gain a basic understanding of how to build connections
between tables, and that made learning new tools more straightforward.
Later in my career, when I started working with MySQL,
I was already able to recognize the underlying principles.
Now it's possible that you'll choose the tools you'll be using.
If that's the case, you'll want to consider the KPIs,
how your stakeholders want to view the data, and how the data needs to be moved.
As you've learned, a KPI is a quantifiable value closely
linked to the business strategy, which is used to track progress toward a goal.
KPIs let us know whether or not we're succeeding, so
that we can adjust our processes to better reach objectives.
For example, some financial KPIs are gross profit margin,
net profit margin, and return on assets.
Or some HR KPIs are rate of promotion and employee satisfaction.
Understanding your organization's KPIs means you can
select tools based on those needs.
Next, depending on how your stakeholders want to view the data,
there are different tools you can choose.
Stakeholders might ask for graphs, static reports, or dashboards.
There are a variety of tools, including Looker Studio, Microsoft, PowerBI and
Tableau.
Some others are Azura Analysis Service, CloudSQL, Pentaho,
SSAS, and SSRS SQL Server, which all have reporting tools built in.
That's a lot of options.
You'll get more insights about these different tools later on.
After you've thought about how your stakeholders want to view the data,
you'll want to consider your back-end tools.
This is when you think about how the data needs to be moved.
For example, not all BI tools can read data lakes.
So, if your organization uses data lakes to store data,
then you need to make sure you choose a tool that can do that.
Some other important considerations when choosing your back-end tools include how
to transfer the data, how it should be updated, and
how the pipeline combines with other tools in the data transformation process.

Each of these points helps you determine must haves for your toolset,
which leads to the best options.
Also, it's important to know that you might end up using a combination of tools
to create the ideal system.
As you've been learning, BI tools have common features, so the skills you learn
in these courses can be used no matter which tools you end up working with.
Going back to my example,
I was able to understand the logic behind transforming and combining tables.
Whether I was using Microsoft Access or MySQL.
This foundation has transferred across the different BI tools I've encountered
throughout my career.
Coming up,
you'll learn more about the solutions that you might work with in the future.
You'll also start getting hands on with some data soon. 


## Business intelligence tools and their applications

As you advance in your business intelligence career, you will encounter many different tools. One of the great things about the skills you have been learning in these courses is that they’re transferable between different solutions. No matter which tools you end up using, the overall logic and processes will be similar! This reading provides an overview of many of these business intelligence solutions.

- Azure Analysis Service (AAS)
	
        Connect to a variety of data sources
        Build in data security protocols
        Grant access and assign roles cross-team
        Automate basic processes

- CloudSQL
	
        Connect to existing MySQL, PostgreSQL or SQL Server databases
        Automate basic processes
        Integrate with existing apps and Google Cloud services, including BigQuery
        Observe database processes and make changes

- Looker Studio
	
        Visualize data with customizable charts and tables
        Connect to a variety of data sources
        Share insights internally with stakeholders and online
        Collaborate cross-team to generate reports
        Use report templates to speed up your reporting

- Microsoft PowerBI
	
        Connect to multiple data sources and develop detailed models
        Create personalized reports
        Use AI to get fast answers using conversational languages
        Collaborate cross-team to generate and share insights on Microsoft applications

- Pentaho
	
        Develop pipelines with a codeless interface
        Connect to live data sources for updated reports
        Establish connections to an expanded library
        Access an integrated data science toolkit

- SSAS SQL Server
	
        Access and analyze data across multiple online databases
        Integrate with existing Microsoft services including BI and data warehousing tools and SSRS SQL Server
        Use built-in reporting tools

- Tableau
	
        Connect and visualize data quickly
        Analyze data without technical programming languages
        Connect to a variety of data sources including spreadsheets, databases, and cloud sources
        Combine multiple views of the data in intuitive dashboards
        Build in live connections with updating data sources


## ETL-specific tools and their applications

In a previous reading, you were given a list of common business intelligence tools and some of their uses. Many of them have built-in pipeline functionality, but there are a few ETL-specific tools you may encounter. Creating pipeline systems—including ETL pipelines that move and transform data between different data sources to the target database—is a large part of a BI professional's job, so having an idea of what tools are out there can be really useful. This reading provides an overview.

- Apache Nifi
	
        Connect a variety of data sources
        Access a web-based user interface
        Configure and change pipeline systems as needed
        Modify data movement through the system at any time

- Google DataFlow
	
        Synchronize or replicate data across a variety of data sources
        Identify pipeline issues with smart diagnostic features
        Use SQL to develop pipelines from the BigQuery UI
        Schedule resources to reduce batch processing costs
        Use pipeline templates to kickstart the pipeline creation process and share systems across your organization

- IBM InfoSphere Information Server
	
        Integrate data across multiple systems
        Govern and explore available data
        Improve business alignment and processes
        Analyze and monitor data from multiple data sources

- Microsoft SQL SIS
	
        Connect data from a variety of sources integration
        Use built-in transformation tools
        Access graphical tools to create solutions without coding
        Generate custom packages to address specific business needs

- Oracle Data Integrator
	
        Connect data from a variety of sources
        Track changes and monitor system performance with built-in features
        Access system monitoring and drill-down capabilities
        Reduce monitoring costs with access to built-in Oracle services

- Pentaho Data Integrator
	
        Connect data from a variety of sources
        Create codeless pipelines with drag-and-drop interface
        Access dataflow templates for easy use
        Analyze data with integrated tools

- Talend
    	
        Connect data from a variety of sources
        Design, implement, and reuse pipeline from a cloud server
        Access and search for data using integrated Talend services
        Clean and prepare data with built-in tools



# DATA-PROCESSING WITH DATAFLOW

## Introduction to Dataflow

Recently, you're introduced to data pipelines.
You learn that many of the procedures and understandings involved in one pipeline
tool can be transferred to other solutions.
So in this course we're going to be using Google Dataflow.
But even if you end up working with a different pipeline tool, the skills and
steps involved here will be very useful.
And using Google Dataflow now will be a great opportunity to practice
everything you've learned so far.
We'll start by introducing you to data flow and going over its basic utilities.
Later on you'll use this tool to complete some basic BI tasks and
set up your own pipeline.
Google Data Flow is a serverless data-processing service that reads data
from the source, transforms it, and writes it in the destination location.
Dataflow creates pipelines with open source libraries which you can interact
with using different languages including Python and SQL.
Dataflow includes a selection of pre-built templates that you can customize or
you can use SQL statements to build your own pipelines.
The tool also includes security features to help keep your data safe.
Okay, let's open Dataflow and explore it together now.
First, we'll log in and go to the console.
Once the console is open, let's find the jobs page.
If this is your first time using Dataflow, it will say no jobs to display.
The jobs page is where we'll find current jobs in our project space.
There are options to create jobs from template or create jobs from SQL.
Snapshot save the current state of a streaming pipeline so
that you can start a new version without losing the current one.
This is great for testing your pipelines, updating them seamlessly for users and
backing up and recovering old versions.
The pipeline section contains a list of the pipelines you've created.
Again, if this is your first time using data flow, it will display the processes
you need to enable before you can start building pipelines.
Now is a great time to do that.
Just click fix all to enable the API features and set your location. 


## Guide to Dataflow

As you have been learning, Dataflow is a serverless data-processing service that reads data from the source, transforms it, and writes it in the destination location. Dataflow creates pipelines with open source libraries, with which you can interact using different languages, including Python and SQL. This reading provides information about accessing Dataflow and its functionality. 

- Navigate the homepage

Go to the Dataflow Google Cloud homepage and sign in to your account to access Dataflow. Then click  the Go to Console button or the Console button. Here, you will be able to create new jobs and access Dataflow tools.

- Jobs 

When you first open the console, you will find the Jobs page. The Jobs page is where your current jobs are in your project space. There are also options to CREATE JOB FROM TEMPLATE or CREATE MANAGED DATA PIPELINE from this page, so that you can get started on a new project in your Dataflow console. This is where you will go anytime you want to start something new. 

- Pipelines

Open the menu pane to navigate through the console and find the other pages in Dataflow. The Pipelines menu contains a list of all the pipelines you have created. If this is your first time using Dataflow, it will also display the processes you need to enable before you can start building pipelines. If you haven’t already enabled the APIs, click Fix All to enable the API features and set your location. 

- Workbench 

The Workbench section is where you can create and save shareable Jupyter notebooks with live code. This is helpful for first-time ETL tool users to check out examples and visualize the transformations. 

- Snapshots

Snapshots save the current state of a pipeline to create new versions without losing the current state. This is useful when you are testing or updating current pipelines so that you aren’t disrupting the system. This feature also allows you to back up and recover old project versions. You may need to enable APIs to view the Snapshots page; you will learn more about APIs in an upcoming activity. 

- SQL Workspace

Finally, the SQL Workspace is where you interact with your Dataflow jobs, connect to BigQuery functionality, and write necessary SQL queries for your pipelines.

Dataflow also gives you the option to interact with your databases using other coding languages, but you will primarily be using SQL for these courses.

_Dataflow is a valuable way to start building pipelines and exercise some of the skills you have been learning in this course. Coming up, you will have more opportunities to work with Dataflow, so now is a great time to get familiar with the interface!_


## Coding with Python

If you're coming into these courses from
the Google Data Analytics Certificate,
or if you've been working with relational databases,
you're probably familiar with the query language, SQL.
Query languages are
specific computer programming languages
used to communicate with a database.
As a BI professional,
you may be expected to use
other kinds of programming languages too.
That's why in this video,
we'll explore one of
the most popular programming languages
out there, Python.
A programming language is a system of words and
symbols used to write instructions that computers follow.
There are lots of different programming languages,
but Python was specifically developed to enable users to
write commands in fewer lines than most other languages.
Python is also open source,
which means it's freely available and may
be modified and shared by the people who use it.
There's a large community of Python users who
develop tools and libraries to make Python better,
which means there are a lot of resources
available for BI professionals to tap into.
Python is a general purpose programming language
that can be applied to a variety of contexts.
In business intelligence, it's used to connect to
a database system to read and modify files.
It can also be combined with
other software tools to develop
pipelines and it can
even process big data and perform calculations.
There are a few key things you should understand
about Python as you begin your programming journey.
First, it is primarily object-oriented and interpreted.
Let's first understand what it
means to be object-oriented.
Object-oriented programming languages are
modeled around data objects.
These objects are chunks of
code that capture certain information.
Basically, everything in the system is an object,
and once data has been captured within the code,
it's labeled and defined by the system so that
it can be used again later
without having to re-enter the data.
Because Python has been adopted
pretty broadly by the data community,
a lot of libraries have been
developed to pre-define data structures
and common operations that
you can apply to the objects in your system.
This is extremely useful when you need to repeat
analysis or even use
the same transformations for multiple projects.
Not having to re-enter the code from scratch saves time.
Note that object-oriented programming languages
differ from functional programming languages,
which are modeled around functions.
While Python is primarily object-oriented,
it can also be used as
a functional programming language
to create and apply functions.
Part of the reason Python is so
popular is that it's flexible.
But for BI,
the really valuable thing about Python is its ability to
create and save data objects
that can then be interacted with via code.
Now, let's consider the fact that
Python is an interpreted language.
Interpreted languages are programming languages
that use an interpreter;
typically another program to
read and execute coded instructions.
This is different from a compiled programming language,
which compiles coded instructions
that are executed directly by the target machine.
One of the biggest differences between
these two types of programming languages is that
the compiled code executed by
the machine is almost impossible for humans to read.
So Python's interpreted language,
it's very useful for BI professionals because
it enables them to use language in an interactive way.
For example, Python can be used to make notebooks.
A notebook is an interactive,
editable programming environment
for creating data reports.
This can be a great way to build
dynamic reports for stakeholders.
Python is a great tool to have in your BI toolbox.
There's even an option to use
Python commands in Google Dataflow.
Pretty soon, you'll get to
check it out for yourself when you
start writing Python in your Dataflow workspace. 


## Python applications and resources

In this course, you will primarily be using BigQuery and SQL when interacting with databases in Google DataFlow. However, DataFlow does have the option for you to work with Python, which is a widely used general-purpose programming language. Python can be a great tool for business intelligence professionals, so this reading provides resources and information for adding Python to your toolbox!

- Elements of Python

There are a few key elements about Python that are important to understand:

    Python is open source and freely available to the public.

    It is an interpreted programming language, which means it uses another program to read and execute coded instructions.

    Data is stored in data frames, similar to R.

    In BI, Python can be used to connect to a database system to work with files.

    It is primarily object-oriented.

    Formulas, functions, and multiple libraries are readily available.

    A community of developers exists for online code support.

    Python uses simple syntax for straightforward coding.

    It integrates with cloud platforms including Google Cloud, Amazon Web Services, and Azure.

- Resources

If you’re interested in learning Python, there are many resources available to help. Here are just a few:

    The Python Software Foundation (PSF): a website with guides to help you get started as a beginner

    Python Tutorial: a Python 3 tutorial from the PSF site

    Coding Club Python Tutorials: a collection of coding tutorials for Python

- General tips for learning programming languages

As you have been discovering, there are often transferable skills you can apply to a lot of different tools—and that includes programming languages! Here are a few tips:

    Define a practice project and use the language to help you complete it. This makes the learning process more practical and engaging.

    Keep in mind previous concepts and coding principles. After you have learned one language, learning another tends to be much easier.

    Take good notes or make cheat sheets in whatever format (handwritten or typed) that works best for you.

    Create an online filing system for information that you can easily access while you work in various programming environments.



# ORGANIZE DATA IN BIGQUERY

## Gather information from stakeholders

You've already learned quite a bit
about the different stakeholders that a BI
professional might work with in
an organization and how to communicate with them.
You've also learned that
gathering information from stakeholders at
the beginning of a project is
an essential step of the process.
Now that you understand more about pipelines,
let's consider what information you need to gather from
stakeholders before building BI processes for them,
that way you'll know exactly what they need
and can help make their work as efficient as possible.
Part of your job as a BI professional
is understanding the current processes in
place and how you can integrate
BI tools into those existing workstreams.
Oftentimes in BI,
you aren't just trying to answer
individual questions every day,
you're trying to find out what questions
your team is asking so
that you can build them a tool that enables
them to get that information themselves.
It's rare for people to know exactly what
they need and communicate that to you.
Instead, they will usually come to
you with a list of problems or symptoms,
and it's your responsibility
to figure out how to help them.
Stakeholders who are less familiar with data
simply don't know what BI processes are possible.
This is why cross business alignment is so important.
You want to create a user-centered design where
all of the requirements for the entire team are met,
that way your solutions address everyone's needs at once,
streamlining their processes as a group.
It can be challenging to figure out what
all of your different stakeholders require.
One option is to create a presentation
and lead a workshop session with the different teams.
This can be a great way to support
cross business alignment and determine everyone's needs.
It's also very helpful to spend some time observing
your stakeholders at work and asking
them questions about what they're doing and why.
In addition, it's important to
establish the metrics and what data
the target table should contain
early on with cross team stakeholders.
This should be done before you start building the tools.
As you've learned, a metric is
a single quantifiable data point
that is used to evaluate performance.
In BI, the metrics businesses
are usually interested in are
KPIs that help them assess how
successful they are at achieving certain goals.
Understanding those goals and how they can be
measured is an important first step
in building a BI tool.
You also know that target tables are
the final destination where data is acted on.
Understanding the end goals
helps you design the best process.
It's important to remember that building
BI processes is a collaborative and iterative process.
You will continue gathering
information from your stakeholders and
using what you've learned until you
create a system that works for your team,
and even then you might change it as new needs arise.
Often, your stakeholders
will have identified their questions,
but they may not have identified
their assumptions or biases about the project yet.
This is where a BI professional can offer insights.
Collaborating closely with stakeholders
ensures that you are keeping their needs in
mind as you design
the BI tools that will streamline their processes.
Understanding their goals, metrics,
and final target tables,
and communicating across multiple teams
will ensure that you make systems that work for everyone.


## Merge data from multiple sources with BigQuery

Previously, you started exploring Google Dataflow, a Google Cloud Platform (GCP) tool that reads data from the source, transforms it, and writes it in the destination location. In this lesson, you will begin working with another GCP data-processing tool: BigQuery. As you may recall from the Google Data Analytics Certificate, BigQuery is a data warehouse used to query and filter large datasets, aggregate results, and perform complex operations.

As a business intelligence (BI) professional, you will need to gather and organize data from stakeholders across multiple teams. BigQuery allows you to merge data from multiple sources into a target table. The target table can then be turned into a dashboard, which makes the data easier for stakeholders to understand and analyze. In this reading, you will review a scenario in which a BI professional uses BigQuery to merge data from multiple stakeholders in order to answer important business questions.

- The problem

Consider a scenario in which a BI professional, Aviva, is working for a fictitious coffee shop chain. Each year, the cafes offer a variety of seasonal menu items. Company leaders are interested in identifying the most popular and profitable items on their seasonal menus so that they can make more confident decisions about pricing; strategic promotion; and retaining, expanding, or discontinuing menu items.

- The solution

1. Data extraction:

In order to obtain the information the stakeholders are interested in, Aviva begins extracting the data. The data extraction process includes locating and identifying relevant data, then preparing it to be transformed and loaded. To identify the necessary data, Aviva implements the following strategies:

2. Meet with key stakeholders

Aviva leads a workshop with stakeholders to identify their objectives. During this workshop, she asks stakeholders questions to learn about their needs:

    What information needs to be obtained from the data (for instance, performance of different menu items at different restaurant locations)?

    What specific metrics should be measured (sales metrics, marketing metrics, product performance metrics)?

    What sources of data should be used (sales numbers, customer feedback, point of sales)?

    Who needs access to this data (management, market analysts)?

    How will key stakeholders use this data (for example, to determine which items to include on upcoming menus, make pricing decisions)?

3. Observe teams in action

Aviva also spends time observing the stakeholders at work and asking them questions about what they’re doing and why. This helps her connect the goals of the project with the organization’s larger initiatives. During these observations, she asks questions about why certain information and activities are important for the organization.

4. Organize data in BigQuery

Once Aviva has completed the data extraction process, she transforms the data she’s gathered from different stakeholders and loads it into BigQuery. Then she uses BigQuery to design a target table to organize the data. The target table helps Aviva unify the data. She then uses the target table to develop a final dashboard for stakeholders to review. 

- The results

When stakeholders review the dashboard, they are able to identify several key findings about the popularity and profitability of items on their seasonal menus. For example, the data indicates that many peppermint-based products on their menus have decreased in popularity over the past few years, while cinnamon-based products have increased in popularity. This finding leads stakeholders to decide to retire three of their peppermint-based drinks and bakery items. They also decide to add a selection of new cinnamon-based offerings and launch a campaign to promote these items. 

- Key findings

Organizing data from multiple sources in a tool like BigQuery allows BI professionals to find answers to business questions. Consolidating the data in a target table also makes it easier to develop a dashboard for stakeholders to review. When stakeholders can access and understand the data, they can make more informed decisions about how to improve services or products and take advantage of new opportunities. 


## Unify data with target tables

As you have been learning, target tables are predetermined locations where pipeline data is sent in order to be acted on in a database system. Essentially, a source table is where data comes from, and a target table is where it’s going. This reading provides more information about the data-extraction process and how target tables fit into the greater logic of business intelligence processes.

- Data extraction

Data extraction is the process of taking data from a source system, such as a database or a SaaS, so that it can be delivered to a destination system for analysis. You might recognize this as the first step in an ETL (extract, transform, and load) pipeline. There are three primary ways that pipelines can extract data from a source in order to deliver it to a target table:

    Update notification: The source system issues a notification when a record has been updated, which triggers the extraction.

    Incremental extraction: The BI system checks for any data that has changed at the source and ingests these updates.

    Full extraction: The BI system extracts a whole table into the target database system.

Once data is extracted, it must be loaded into target tables for use. In order to drive intelligent business decisions, users need access to data that is current, clean, and usable. This is why it is important for BI professionals to design target tables that can hold all of the information required to answer business questions.

- The importance of target tables

As a BI professional, you will want to take advantage of target tables as a way to unify your data and make it accessible to users. In order to draw insights from a variety of different sources, having a place that contains all of the data from those sources is essential.


## Activity: Create a target table in BigQuery

In this activity, you used BigQuery to create a target table to store data you pulled from a dataset of street tree information from San Francisco, California. In your BI role, you’ll need to use programs such as BigQuery and Dataflow to move and analyze data with SQL. Now, you’ve practiced a key part of the Extraction stage of the BI pipeline: pulling data from a source and placing it into its own table.

To explore the query result exemplar, download the following attachment: CSV File "SanFranciscoTrees"

- ASSESSMENT

In this activity, you ran the following SQL query to create a target table:

    SELECT
        address,
        COUNT(address) AS number_of_trees
    FROM
        `bigquery-public-data.san_francisco_trees.street_trees`
    WHERE
        address != "null"
    GROUP BY address
    ORDER BY number_of_trees DESC
    LIMIT 10;

The SELECT clause selects the address of each tree. By using the COUNT function, you count the number of trees at each address and return a single row of data per address, instead of per tree. This data is saved as a new column.

The FROM clause is straightforward as it specifies the street_trees table within the San Francisco Street Trees dataset. 

The WHERE clause is necessary to ensure that your target table only includes rows that have a value in the address column. 

The GROUP BY clause specifies that you’re grouping data by the address, and the ORDER BY clause sorts the data in descending order by number_of_trees column.

The LIMIT clause limits the query to return only the top ten rows of data. When working with large datasets, including a limit will decrease the processing time required to return the data. 

- RESULT

The result of this query is a target table with two columns. It features the address column, as well as the total number of trees planted at the address you calculated in the SELECT clause. If properly executed, the first value in the address column is 100x Cargo Way. Next to it, the number_of_trees is 135. If you didn’t receive this result, please review the code and run it again.

Furthermore, the target table shows the 10 addresses with the most trees planted by the Department of Public Works in the city of San Francisco:

    100x Cargo Way
    700 Junipero Serra Blvd
    1000 San Jose Ave
    1200 Sunset Blvd
    1600 Sunset Blvd
    2301 Sunset Blvd
    1501 Sunset Blvd
    2401 Sunset Blvd
    100 STAIRWAY5
    2601 Sunset blvd

And the number of trees for each address is as follows:

    100x Cargo Way: 135
    700 Junipero Serra Blvd: 125
    1000 San Jose Ave: 113
    1200 Sunset Blvd: 110
    1600 Sunset Blvd: 102
    2301 Sunset Blvd: 94
    1501 Sunset Blvd: 93
    2401 Sunset Blvd: 92
    100 STAIRWAY5: 87
    2601 Sunset Blvd: 84

- Key takeaways:

Target tables are the destination for data during the Extraction stage of a pipeline. You’ll use them in your role as a BI professional to store data after pulling it from their sources. Once they’re in a target table, you can transform them with BigQuery or Dataflow and load them into reporting tables. You’ll learn about the Transform and Load stages of data pipelines later in this course.


## Case study: Wayfair - Working with stakeholders to create a pipeline

Working with stakeholders while designing and iterating on a pipeline system is an important strategy for ensuring that the BI systems you put in place answer their business needs. In this case study, you’ll discover how the BI team at e-commerce home retailer Wayfair, headquartered in Boston, Massachusetts, works with their stakeholders throughout a project to create a pipeline system that works for them.

- Company background:

Longtime friends Niraj Shah and Steve Conine started the online-only company in 2002 after deciding they wanted to offer a larger selection of choices to customers—more than could fit in a brick-and-mortar space. They started the company as a collection of more than 200 e-commerce stores, each selling separate categories of products. In 2011, the company combined these sites to establish wayfair.com.

Wayfair is now one of the world’s largest home retailers. The company’s goal is to help everyone, anywhere, create their feeling of home. It empowers customers to create spaces that reflect who they are, what they need, and what they value.

- The challenge:

The Wayfair pricing ecosystem includes thousands of different inputs and outputs across a full catalog of products, which change multiple times a day. All of these inputs and outputs are being generated in different ways from different sources. Because of this, the BI team and other data professionals who needed to access pricing data were having trouble locating, querying, and interpreting the complete dataset. This led to incomplete and often inaccurate insights that weren’t useful for decision makers. 

To address this, the BI team decided to design and implement a new pipeline system to consolidate all the data stakeholders needed. They also needed to consider a few additional challenges with their pipeline system:

    Monitoring and reporting around these processes would need to be included in the design to track and manage errors.

    Data would need to be clean before it could be shared with downstream users. 

    Due to the variety of data types being joined, the BI team also needed to better understand the data relationships so they could accurately consolidate the data. 

    Training sessions would be required to help educate users on how to best access and use the new datasets. 

These unique challenges meant that it was especially important for the BI team to work closely with stakeholders while developing their new system to address their needs and create something that worked across multiple teams. 

- The approach:

Given the massive amount of data within the system, it was important for the BI team to step back and work with stakeholders to really understand how they were using the data currently. That included understanding the business problems they were trying to solve, the data they were already using and how they were accessing it, and the data they wanted to use but couldn’t access yet. 

Once they had communicated with stakeholders, the team was able to design a pipeline that achieved three key goals:

    All the required data could be made available and easy to understand and use

    The system was more efficient and could make data available without delays

    The system was designed to scale as the dataset expanded vertically and horizontally to support future growth

After this initial design was completed, the system was presented to stakeholders for review to ensure they understood the system and that it met all of their needs. This project required collaboration across a variety of stakeholders and teams:

    Software engineers: The software engineer team were the primary owners and generators of data, so they were key to understanding the current state of the data and helped make it accessible for the BI team to work with.

    Data architects: The BI team consulted with data architects to ensure that the pipeline design was all-encompassing, efficient, and scalable so the BI team could handle the amount of data being ingested by the system and ensure that downstream users would have access to the data as the system was being scaled. 

    Data professionals: As the core users, these teams provided the use cases and requirements for the system so that the BI team could ensure that the pipeline addressed their needs. Because each of their respective teams’ needs were different, it was important to ensure the system design and data included was wide enough to account for all of those needs. 

    Business stakeholders: As the end users of the insights generated by the entire pipeline, the business stakeholders ensured all development work and use cases were rooted with clear business problems to ensure what the BI team built could be immediately applied to their work. 

Communicating with all of the stakeholders throughout the design process ensured that the Wayfair BI team created something useful and long-lasting for their organization.

- The results:

The final pipeline that the BI team implemented achieved a variety of key goals for the entire organization:

    It enabled software engineering teams to publish data in real-time for the BI team to use.

    It consolidated the different data components into one unified dataset for ease of access and use.

    It allowed the BI team to store different data components in their own individual staging layers.

    It included additional processes to monitor and report on the system’s performance to inform users where failures were occurring and enable quick fixes.

    It created a unified dataset that users could leverage to build metrics and report on data.

The greatest benefit of this pipeline solution was that Wayfair now had the ability to provide accurate information in one place for users, eliminating the need to join different sources themselves. This meant that the team could promote more accurate insights for stakeholders and get rid of costly ad-hoc processes. 

The response cross-team was very positive. The director of analytics at Wayfair said that this was revolutionary for their team’s daily work because they had information on retail price, cost inputs, and product status in the same place for the first time. This was a huge benefit for their processes and to help them handle their data in a more intelligent way. 

- Conclusion:

A significant benefit that business intelligence provides an organization is that it makes the systems and processes more efficient and effective for users across the organization; basically, BI makes everyone’s jobs a little easier. Ensuring that the BI team is tightly aligned with the business stakeholders and other teams is critical to their success. Without great partnership, problems can’t be solved correctly. 



# REVIEW: DATA MODELS & PIPELINES

## Wrap-up

Hey, great work so far.
You're almost done with the first section of
this course. You've learned a lot.
So far, we've discussed
a BI professional's role in
the organization and storage of data.
You also investigated data models and schemas,
how BI professionals develop
design patterns based on the organization's needs,
and how databases are designed.
You've been introduced to data pipelines, ETL processes,
and building BI tools that help automate moving
data from storage systems to target destinations.
You've even started using tools to
begin building your own pipelines.
Finally, you learned strategies
for gathering information from
stakeholders to ensure that the tools you
create for them actually solve the business problems.
But creating systems that manage and move data
is just one part of a BI professional's job.
You also have to make sure that those systems
continue working for your stakeholders.
Coming up, you're going to discover how to
maintain your BI tools and optimized database systems.
I hope you're excited to learn
more because there's a lot
more I wanted to share with you.
But first, you have another challenge ahead.
Feel free to spend some time with the glossary and review
any of the section's content
before moving on to your next assessment.
Then I'll be here when you're ready to take next step. 


## Glossary

Attribute: In a dimensional model, a characteristic or quality used to describe a dimension

Columnar database: A database organized by columns instead of rows

Combined systems: Database systems that store and analyze data in the same place

Compiled programming language: A programming language that compiles coded instructions that are executed directly by the target machine

Data lake: A database system that stores large amounts of raw data in its original format until it’s needed

Data mart: A subject-oriented database that can be a subset of a larger data warehouse

Data warehouse: A specific type of database that consolidates data from multiple source systems for data consistency, accuracy, and efficient access

Database migration: Moving data from one source platform to another target database

Dimension (data modeling): A piece of information that provides more detail and context regarding a fact

Dimension table: The table where the attributes of the dimensions of a fact are stored

Design pattern: A solution that uses relevant measures and facts to create a model in support of business needs

Dimensional model: A type of relational model that has been optimized to quickly retrieve data from a data warehouse

Distributed database: A collection of data systems distributed across multiple physical locations

Fact: In a dimensional model, a measurement or metric

Fact table: A table that contains measurements or metrics related to a particular event

Foreign key: A field within a database table that is a primary key in another table (Refer to primary key)

Functional programming language: A programming language modeled around functions

Google DataFlow: A serverless data-processing service that reads data from the source, transforms it, and writes it in the destination location

Interpreted programming language: A programming language that uses an interpreter, typically another program, to read and execute coded instructions

Logical data modeling: Representing different tables in the physical data model

Object-oriented programming language: A programming language modeled around data objects

OLAP (Online Analytical Processing) system: A tool that has been optimized for analysis in addition to processing and can analyze data from multiple databases

OLTP (Online Transaction Processing) database: A type of database that has been optimized for data processing instead of analysis

Primary key: An identifier in a database that references a column or a group of columns in which each row uniquely identifies each record in the table (Refer to foreign key)

Python: A general purpose programming language

Response time: The time it takes for a database to complete a user request

Row-based database: A database that is organized by rows

Separated storage and computing systems: Databases where data is stored remotely, and relevant data is stored locally for analysis

Single-homed database: Database where all of the data is stored in the same physical location

Snowflake schema: An extension of a star schema with additional dimensions and, often, subdimensions

Star schema: A schema consisting of one fact table that references any number of dimension tables

Target table: The predetermined location where pipeline data is sent in order to be acted on



# REVIEW: DATA ANALYTICS CONTENT

## Data types

I don't know about you, but when
I'm choosing a movie to watch,
I sometimes get stuck between a couple of choices.
If I'm in the mood for excitement or suspense,
I might go for a thriller,
but if I need a good laugh,
I'll choose a comedy.
If I really can't decide between two movies,
I might even use some of my data analysis skills
to compare and contrast them.
Come to think of it, there really needs to be
more movies about data analysts, I'd watch that.
But since we can't watch a movie about data,
at least not yet, we'll do the next best thing,
watch data about movies.
We're going to take a look at
this spreadsheet with movie data.
We know we can compare
different movies and movie genres,
turns out, you can do the same with
data and data formats.
Let's use our movie data spreadsheet
to understand how that works.
We'll start with quantitative and qualitative data.
If we check out column A,
we'll find titles of the movies.
This is qualitative data because it can't be counted,
measured, or easily expressed using numbers.
Qualitative data is usually listed as
a name, category, or description.
In our spreadsheet, the movie titles and
cast members or qualitative data.
Next up is quantitative data,
which can be measured or
counted and then expressed as a number.
This is data with a certain quantity, amount, or range.
In our spreadsheet here,
the last two columns show
the movie's budget and box office revenue.
The data in these columns is listed in dollars,
which can be counted,
so we know that data is quantitative.
We can go even deeper into quantitative data
and break it down into discrete or continuous data.
Let's check out discrete data first.
This is data that's counted
and has a limited number of values.
Going back to our spreadsheet,
we'll find each movie's budget and
box office returns in columns
M and N. These are both examples of discrete data,
they can be counted and have a limited number of values.
For example, the amount of money
a movie makes can only be represented
with exactly two digits after
the decimal to represent sense,
there can be anything between one and two cents.
Continuous data can be measured using a timer and
its value can be shown as a decimal with several places.
Let's imagine a movie about data analysts
that I'm definitely going to star in someday,
you could express that movie's run-time as
110.0356 minutes. You could even add fractional data
after the decimal point if you needed to.
There's also nominal and ordinal data.
Nominal data is a type of
qualitative data that's categorized without a set order,
in other words, this data doesn't have a sequence.
Here's a quick example,
let's say you're collecting data about movies,
you ask people if they've watched a given movie,
their responses would be in the form of nominal data.
They could respond yes,
no, or not sure.
These choices don't have a particular order.
Ordinal data, on the other hand,
is a type of qualitative data with a set order or scale.
If you asked a group of people to rank a movie from 1-5,
some might rank it as a two,
others a four, and so on.
These rankings are in order of how
much each person liked the movie.
Let's talk about internal data,
which is data that lives within a company's own systems.
For example, if a movie studio had compiled all of
the data in the spreadsheet using
only their own collection methods,
then it would be their internal data.
The great thing about internal data is that it's
usually more reliable and easier to collect.
But in the spreadsheet,
it's more likely that the movie studio
had to use data owned or shared
by other studios and
sources because it includes movies they didn't make.
That means they'd be collecting external data.
External data is, you guessed it,
data that lives and is
generated outside of an organization.
External data becomes particularly valuable when
your analysis depends on as many sources as possible.
A great thing about this data is that it's structured.
Structured data is data
that's organized in a certain format,
such as rows and columns.
Spreadsheets and relational databases are
two examples of software
that can store data in a structured way.
You might remember our earlier exploration
of structured thinking,
which helps you add a framework to a problem so that
you can solve it in an organized and logical manner,
you can think of structured data in the same way.
Having a framework for the data makes the data
easily searchable and more analysis-ready.
As a data analyst,
you'll work with a lot of structured data,
which will usually be in the form of
a table spreadsheet or relational database.
But sometimes you'll come across unstructured data.
This is data that is not organized in
any easily identifiable manner.
Audio and video files are examples of unstructured data
because there's no clear way to
identify or organize their content.
Unstructured data might have internal structure,
but the data doesn't fit neatly in rows and
columns like structured data. There you have it.
Hopefully, you're now more familiar with
data formats and how you might use them in your work.
In just a bit,
you'll continue to explore structured data and learn
even more about the data you'll
use most often as an analyst.
Coming soon to a screen near you. 


## Primary and foreign keys

Databases are essential tools for data analysts.
I use them constantly.
Just about all of the data I
access is stored within databases.
Databases store and organize data,
making it much easier for data
analysts to manage and access information.
They help us get insights faster,
make data-driven decisions, and solve problems.
You've already heard a bit about what databases
are and how they're used by data analysts.
Now let's learn more about
database features and components.
Here's a simple database structure.
It contains tables with
information from a car manufacturer.
The top level includes car dealerships,
product details, and repair parts.
Then if you drill down to
the next level by selecting one of those tables,
you'll find more specific details about each item.
This is called a relational database.
A relational database is
a database that contains a series
of related tables that can be
connected via their relationships.
For two tables to have a relationship,
one or more of the same fields
must exist inside both tables.
For example, here,
branch ID exists in this table and this one.
If a field exists within both tables,
we can use it to connect the tables together.
The branch ID field is
the key to connecting these tables.
There are two types of keys.
A primary key is an identifier that
references a column in which each value is unique.
You can think of it as the unique identifier
for each row in a table.
For our dealership table with
information about the different dealership branches,
branch ID is the primary key.
Similarly, for the product details table about each car,
VIN is our primary key.
As an analyst, you may need to create tables.
If you do decide to include a primary key,
it should be unique, meaning
no two rows can have the same primary key.
Also, it cannot be null or blank.
There are also foreign keys.
A foreign key is a field within
a table that's a primary key in another table.
In other words, a foreign key is
how one table can be connected to another.
Because I repair parts table
contains information about each car part,
the primary key is part ID.
Each row in our repair parts table
represents one unique part.
All the other keys in this table, such as the VIN,
are the foreign keys that allow
the repair parts table to
be connected to the other tables.
As you can see, a table can only have one primary key,
but it can have multiple foreign keys.
Understanding primary and foreign keys can be tricky,
so you'll have more opportunities to practice coming up.
But as a general summary,
a primary key is used to ensure
data in a specific column is unique.
It uniquely identifies a record
in a relational database table.
Only one primary key is allowed in a table,
and they cannot contain null or blank values.
And a foreign key is a column or group of columns in
a relational database table that
provides a link between the data in two tables.
It refers to the field in a table that's
the primary key of another table.
Lastly, it's important to note that
more than one foreign key is allowed to exist in a table.
Feel free to re-watch this video to be sure you
understand primary and foreign keys clearly.
Coming up, you'll begin practicing how to
access and analyze data from actual databases.
That will be a great opportunity to improve
your understanding of primary and foreign keys,
database organization, and how you might
use databases in your future analytics career.


## BigQuery

Hey there. In this video,
we're going to learn about each part
of the BigQuery SQL workspace
so you can use it during this course
and throughout your career as a data analyst.
It's an extremely valuable and widely popular tool,
so understanding how it works is super helpful.
Feel free to follow along on
your screen as we explore BigQuery.
You may notice that my screen
appears a little different than
yours, since BigQuery is
constantly updating its interface.
Don't worry if this happens as
minor differences won't stop
you from understanding the basics.
To begin, go to the BigQuery landing page,
then login to the account you created earlier.
To navigate to the SQL workspace,
select the menu on the left side of
the screen and scroll down to the Big Data header.
Then hover over the BigQuery label
and click ''SQL workspace'' from the drop-down.
Now that we're in the SQL workspace,
we're going to search for public datasets,
select a dataset through the Data Explorer,
run a query, and upload our own data for querying.
First, we'll search for a public dataset to use.
To select a public dataset,
navigate to the Explorer menu
on the left side of the screen.
Click the "Add Data" button
in the upper right of the menu.
Then in the drop-down menu,
select "Explore public datasets."
This will open the marketplace and
show you available public datasets.
Let's go to the search marketplace bar and
search for noaa_lightning,
a dataset we'll use in an upcoming activity.
Click on the ''Cloud-to-Ground
Lightning Strikes'' dataset.
This will give us a description and
preview of the dataset which captures
observations about lightning activity
and weather patterns in the United States.
Click "View dataset."
This will bring you back to
the SQL workspace and create a tab for the dataset.
We can then move back to the Editor tab we have opened,
or click "Compose new query" to begin writing with SQL.
On the left, notice that
the BigQuery public data drop-down list
is in the Explorer menu.
We can click the arrow to expand
the BigQuery data list and pick out a new dataset.
Let's select the first dataset in
the drop-down list, austin_311.
When we do, it expands to
show the table within the dataset.
We can open the dataset for a preview.
The Schema tab contains
the names of each column in the dataset.
The Details tab contains additional metadata,
such as the creation date of the dataset.
The Preview tab contains the first rows from the dataset.
On this page, we can click
"Query" to automatically create
a new editor window with
the template for a query already populated.
From here, put an asterisk after Select,
where our cursor pops up,
then run the query.
Congratulations, you ran a SQL query in BigQuery.
The query you ran returned rows from
the dataset which populate in
a window beneath the editor interface.
Results from any query you run will also display here.
Now let's say you have the results
of a survey that you want to
upload to BigQuery and analyze using SQL.
To add your own data to BigQuery,
choose the ID of the project you want to add to.
Select the three vertical dots icon to open
options for the project then choose "Create dataset."
Name the dataset something that will
help you identify it later,
such as upload_test_dataset.
Then click "Create dataset."
Next, go to the Explorer menu and choose
the three vertical dots next to
the dataset under the Projects drop down.
Now we'll select the icon for create table,
which opens a pop-up window.
Under Source and create table from,
select "Upload" or whichever
method you prefer to upload your data.
Here, we can upload any data file,
such as a CSV file.
Let's give our table a helpful name such as test_table.
Make sure that the schema is set to auto
detect and select "Create table."
There's more to come with BigQuery.
Feel free to re-watch this video anytime
and keep practicing. See you soon. 


## SQL best practices

These best practices include guidelines for writing SQL queries, developing documentation, and examples that demonstrate these practices. This is a great resource to have handy when you are using SQL yourself; you can just go straight to the relevant section to review these practices. Think of it like a SQL field guide!

- Capitalization and case sensitivity

With SQL, capitalization usually doesn’t matter. You could write SELECT or select or SeLeCT. They all work! But if you use capitalization as part of a consistent style your queries will  look more professional.

To write SQL queries like a pro, it is always a good idea to use all caps for clause starters (e.g., SELECT, FROM, WHERE, etc.). Functions should also be in all caps (e.g., SUM()). Column names should be all lowercase (refer to the section on snake_case later in this guide). Table names should be in CamelCase (refer to the section on CamelCase later in this guide). This helps keep your queries consistent and easier to read while not impacting the data that will be pulled when you run them. The only time that capitalization does matter is when it is inside quotes (more on quotes below).

Vendors of SQL databases may use slightly different variations of SQL. These variations are called SQL dialects. Some SQL dialects are case sensitive. BigQuery is one of them. Vertica is another. But most, like MySQL, PostgreSQL, and SQL Server, aren’t case sensitive. This means if you searched for country_code = ‘us’, it will return all entries that have 'us', 'uS', 'Us', and 'US'. This isn’t the case with BigQuery. BigQuery is case sensitive, so that same search would only return entries where the country_code is exactly 'us'. If the country_code is 'US', BigQuery wouldn’t return those entries as part of your result.

- Single or double quotes: '' or " "

For the most part, it also doesn’t matter if you use single quotes ' ' or double quotes " " when referring to strings. For example, SELECT is a clause starter. If you put SELECT in quotes like 'SELECT' or "SELECT", then SQL will treat it as a text string. Your query will return an error because your query needs a SELECT clause.

But there are two situations where it does matter what kind of quotes you use:

    When you want strings to be identifiable in any SQL dialect
    When your string contains an apostrophe or quotation marks

Within each SQL dialect there are rules for what is accepted and what isn’t. But a general rule across almost all SQL dialects is to use single quotes for strings. This helps get rid of a lot of confusion. So if we want to reference the country US in a WHERE clause (e.g., country_code = 'US'), then use single quotes around the string 'US'.

The second situation is when your string has quotes inside it. Suppose you have a column of favorite foods in a table called FavoriteFoods and the other column corresponds to each friend.

Friend  /  Favorite_food
Rachel DeSantos  -  Shepherd’s pie
Sujin Lee  -  Tacos
Najil Okoro. -  Spanish paella

You might notice how Rachel’s favorite food contains an apostrophe. If you were to use single quotes in a WHERE clause to find the friend who has this favorite food, it would look like this:
Screenshot of Where Clause query with shepherd's pie in single quotes

This won’t work. If you run this query, you will get an error in return. This is because SQL recognizes a text string as something that starts with a quote 'and ends with another quote '. So in the bad query above,  SQL thinks that the Favorite_food you are looking for is 'Shepherd'. Just 'Shepherd' because the apostrophe in Shepherd's ends the string.

Generally speaking, this should be the only time you would use double quotes instead of single quotes. So your query would look like this instead:
SELECT Friend FROM FavoriteFoods WHERE Favorite_food = "Shepherd's pie"

SQL understands text strings as either starting with a single quote ' or double quote". Since this string starts with double quotes, SQL will expect another double quote to signal the end of the string. This keeps the apostrophe safe, so it will return "Shepherd's pie" and not 'Shepherd'.

- Comments as reminders

As you get more comfortable with SQL, you will be able to read and understand queries at a glance. But it never hurts to have comments in the query to remind yourself of what you are trying to do. And if you share your query, it also helps others understand it.

For example:

You can use # in place of the two dashes, --, in the above query but keep in mind that # isn’t recognized in all SQL dialects (MySQL doesn’t recognize #). So it is best to use -- and be consistent with it. When you add a comment to a query using --, the database query engine will ignore everything in the same line after --. It will continue to process the query starting on the next line.

- Snake_case names for columns

It is important to always make sure that the output of your query has easy-to-understand names. If you create a new column (say from a calculation or from concatenating new fields), the new column will receive a generic default name (e.g., f0). 

For example:
SELECT SUM(tickets), COUNT (tickets), SUM (tickets) AS total_tickets, COUNT (tickets) AS number_of_purchases FROM purchases

The following table features the results of this query:
f0: 8
f1: 4
total_tickets: 8
Number_of_purchases: 4

Results are:
f0  -  8
f1  -  4 
total_tickets  -  8
number_of_purchases  -  4


The first two columns are named f0 and f1 because they weren’t named in the above query. SQL defaults to f0, f1, f2, f3, and so on. We named the last two columns total_tickets and number_of_purchases so these column names show up in the query results. This is why it is always good to give your columns useful names, especially when using functions. After running your query, you want to be able to quickly understand your results, like the last two columns we described in the example.

On top of that, you might notice how the column names have an underscore between the words. Names should never have spaces in them. If 'total_tickets' had a space and looked like 'total tickets' then SQL would rename SUM(tickets) as just 'total'. Because of the space, SQL will use 'total' as the name and won’t understand what you mean by 'tickets'. So, spaces are bad in SQL names. Never use spaces.

The best practice is to use snake_case. This means that 'total tickets', which has a space between the two words, should be written as 'total_tickets' with an underscore instead of a space.

- CamelCase names for tables

You can also use CamelCase capitalization when naming your table. CamelCase capitalization means that you capitalize the start of each word, like a two-humped (Bactrian) camel. So the table TicketsByOccasion uses CamelCase capitalization. Please note that the capitalization of the first word in CamelCase is optional; camelCase is also used. Some people differentiate between the two styles by calling CamelCase,PascalCase, and reserving camelCase for when the first word isn't capitalized, like a one-humped (Dromedary) camel; for example, ticketsByOccasion.

At the end of the day, CamelCase is a style choice. There are other ways you can name your tables, including:

    All lower or upper case, like ticketsbyoccasion or TICKETSBYOCCASION

    With snake_case,  like tickets_by_occasion

Keep in mind, the option with all lowercase or uppercase letters can make it difficult to read your table name, so it isn’t recommended for professional use.

The second option, snake_case, is technically okay. With words separated by underscores, your table name is easy to read, but it can get very long because you are adding the underscores. It also takes more time to write. If you use this table a lot, it can become a chore.

In summary, it is up to you to use snake_case or CamelCase when creating table names. Just make sure your table name is easy to read and consistent. Also be sure to find out if your company has a preferred way of naming their tables. If they do, always go with their naming convention for consistency.

- Indentation

As a general rule, you want to keep the length of each line in a query <= 100 characters. This makes your queries easy to read. 

For example, check out this query with a line with >100 characters:
Screenshot of query
SELECT 
CASE WHEN genre = 'horror' THEN 'Will not watch' WHEN genre = 'documentary' 
THEN 'Will watch alone' ELSE 'Watch with others'  END AS
Watch_category, COUNT(

This query is hard to read and just as hard to troubleshoot or edit. Now, here is a query where we stick to the <= 100 character rule: Screenshot of query

Now it is much easier to understand what you are trying to do in the SELECT clause. Sure, both queries will run without a problem because indentation doesn’t matter in SQL. But proper indentation is still important to keep lines short. And it will be valued by anyone reading your query, including yourself!

- Multi-line comments

If you make comments that take up multiple lines, you can use -- for each line. Or, if you have more than two lines of comments, it might be cleaner and easier is to use /* to start the comment and */ to close the comment. 

For example, you can use the -- method like below:
Screenshot of query
-- Date: September 15, 2020
-- Analyst: Jazmin Cisneros
-- Goal: Count the number of rows in the table
SELECT
	COUNT(*) number of rows -- the * stands for all so count all
FROM
	table

Or, you can use the /* */ method like below:
Screenshot of query
/* 
Date: September 15, 2020
Analyst: Jazmin Cisneros
Goal: Count the number of rows in the table
*/
SELECT
	COUNT(*) AS number_of_rows -- the * stands for all so count all
FROM
	table

In SQL, it doesn’t matter which method you use. SQL ignores comments regardless of what you use: #, --, or /* and */. So it is up to you and your personal preference. The /* and  */ method for multi-line comments usually looks cleaner and helps separate the comments from the query. But there isn’t one right or wrong method.

- SQL text editors

When you join a company, you can expect each company to use their own SQL platform and SQL dialect. The SQL platform they use (e.g., BigQuery, MySQL, or SQL Server) is where you will write and run your SQL queries. But keep in mind that not all SQL platforms provide native script editors to write SQL code. SQL text editors give you an interface where you can write your SQL queries in an easier and color-coded way. In fact, all of the code we have been working with so far was written with an SQL text editor!

- Examples with Sublime Text

If your SQL platform doesn’t have color coding, you might want to think about using a text editor like Sublime Text or Atom. This section shows how SQL is displayed in Sublime Text. Here is a query in Sublime Text:

With Sublime Text, you can also do advanced editing like deleting indents across multiple lines at the same time. For example, suppose your query somehow had indents in the wrong places and looked like this:

This is really hard to read, so you will want to eliminate those indents and start over. In a regular SQL platform, you would have to go into each line and press BACKSPACE to delete each indent per line. But in Sublime, you can get rid of all the indents at the same time by selecting all lines and pressing Command (or CTRL in Windows) + [. This eliminates indents from every line. Then you can select the lines that you want to indent (i.e., lines 2, 4, and 6) by pressing the Command key (or the CTRL key in Windows) and selecting those lines. Then while still holding down the Command key (or the CTRL key in Windows), press  ] to indent lines 2, 4, and 6 at the same time. This will clean up your query and make it look like this instead:

Sublime Text also supports regular expressions. Regular expressions (or regex) can be used to search for and replace string patterns in queries. We won’t cover regular expressions here, but you might want to learn more about them on your own because they are a very powerful tool.

You can begin with these resources:

    Search and replace in Sublime Text
    Regex tutorial (if you don’t know what regular expressions are)
    Regex cheat sheet
