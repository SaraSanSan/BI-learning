# | The Path to Insights: DATA MODELS & PIPELINES |

# OPTIMIZE ETL PROCESSES

You’ll learn about optimization techniques including ETL quality testing, data schema validation, business rule verification, and general performance testing. You’ll also explore data integrity and learn how built-in quality checks defend against potential problems. Finally, you’ll focus on verifying business rules and general performance testing to make sure pipelines meet the intended business need.

Learning Objectives:

    Discover strategies to create an ETL process that works to meet organizational and stakeholder needs and how to maintain an ETL process efficiently.
    Introduce tools used in ETL
    Understand the primary goals of ETL quality testing.
    Understand the primary goals of data schema validation.
    Develop ETL quality testing and data schema validation best practices.
    Identify and implement appropriate test scenarios and checkpoints for QA on data pipelines.
    Explain different methods for QA data in the pipeline.
    Create performance testing scenarios and measure performance throughout the pipeline.
    Verify business rules.
    Perform general performance testing.


## Welcome to module 3

You've learned a lot about how BI professionals
ensure that their organizations'
database systems and tools
continue to be as useful as possible.
This includes evaluating whether
fixes or updates are needed,
and performing optimization when necessary.
Previously, we focused
specifically on optimizing database systems.
Now it's time to explore
optimizing pipelines and ETL processes.
In this section of the course,
you'll learn about ETL quality testing,
data schema validation, verifying
business rules and general performance testing.
Through ETL quality testing,
BI Professionals aim to confirm that data is extracted,
transformed, and loaded to
its destination without any errors or issues.
This is especially important because sometimes
your pipeline might start producing
bad or misleading results.
This can happen when the original sources
are changed without your knowledge.
Also, we'll soon cover data schema validation,
which is used to keep source data
aligned with the target database schema.
A schema mismatch can cause system failures.
This is critical to keeping the ETL running smoothly.
We'll also investigate data integrity and how
built-in quality checks
defend against potential problems.
Finally, we'll focus on verifying business rules and
general performance testing to make sure
the pipeline is fulfilling
the business need it was intended to.
There's a lot to come. So let's begin exploring the
optimization processes for pipelines and ETL. 



# OPTIMIZING PIPELINES & ETL PROCESSES

## The importance of quality testing

You're already familiar with ETL pipelines,
where data is extracted from a source,
transformed while it's being moved,
and then loaded into a destination table
where it can be acted on.
Part of the transformation step in
the ETL process, is quality testing.
In BI, quality testing is a process of checking
data for defects in order to prevent system failures.
The goal is to ensure
the pipeline continues to work properly.
Quality testing can be time-consuming,
but it's extremely important
for an organization's workflow.
Quality testing involves seven validation elements: completeness, consistency,
conformity, accuracy,
redundancy, integrity, and timeliness.
That's a lot of elements to keep in mind,
but we're going to break down each in
this video, starting with completeness.
Also, you may recall some of
these concepts from the Google
Data Analytics certificate.
If you'd like, take a few minutes to
review that content before moving ahead.
Let's start with checking for completeness.
This involves confirming that the data
contains all the desired components or measures.
For example, imagine you're
working with sales data and you
have an ETL pipeline that delivers
monthly data to target tables.
These target tables are used to
generate reports for stakeholders.
If the data being moved through
the pipeline is missing a week of data or
information about one of the best-selling products
or another key metric,
then the calculations used to create
reports won't have complete accurate data.
Next, we have consistency.
You might have learned that in a data analytics context,
consistency deals with the degree to which data is
repeatable from different points of entry or collection.
In BI, it's a bit different.
Here, consistency involves confirming that data
is compatible and in agreement across all systems.
Imagine two systems,
one is an HR database with employee data,
and the other is a payroll system.
If the HR database lists
an employee who either isn't in the payroll system,
or is listed differently there,
that inconsistency could create problems.
Next is conformity.
This element is all about whether
the data fits the required destination format.
Consider sales data in an ETL pipeline.
If the data's being extracted includes dates of sale that
don't match the dates that
the destination table is designed to hold,
that's going to create errors.
Now, accuracy has to do with the data conforming to
the actual entity that's being measured or described.
Another way of thinking about this
is if the data represents real values.
With that in mind, any mistyped entries or errors from
the source are problematic
because they will be reflected in the destination.
Source systems requiring a lot of
manual data entry are more
likely to have issues with accuracy.
If a purchase of
a hamburger was miss entered
as selling for a million dollars,
that's something you need to take care
of before the data is loaded.
If you're using a relational storage database,
ensuring that there isn't any redundancy in the data,
is another important element of quality testing.
In a BI context, redundancy is moving,
transforming, or storing more than the necessary data.
This occurs when the same piece of data
is stored in two or more places.
Moving data through a pipeline requires
processing power, time, and resources.
It's important not to move any more data than you need.
For instance, if client company names
are listed in multiple places,
but are only required to appear in
one place in the destination table,
we wouldn't want to waste
resources on loading that redundant data.
Now we come to integrity.
Integrity concerns the accuracy, completeness,
consistency, and trustworthiness of
data throughout its life cycle.
In quality testing, this often means
checking for any missing
relationships in the data values.
As an example, say
a company sales database is relational,
BI professionals would depend on those relationships to
manipulate data within
the database and to query the data.
Maybe they have product IDs
and descriptions in a database.
But if there's a description and
no corresponding record with the ID,
there's now an issue with data integrity.
It's essential to make sure this is
addressed before moving on to analysis.
Data mapping is one way to make sure that the data from
the source matches the data in the target database.
You'll learn more about this later.
But basically, data mapping is a process of
matching fields from one data source to another.
Last but not least,
you want to make sure your data is timely.
Timeliness involves confirming that data is current.
This check is done specifically to
make sure data has been updated
with the most recent information
that can provide relevant insights.
For example, if a data warehouse
is supposed to contain daily data,
but doesn't update properly then
the pipeline can't ingest the latest information.
BI professionals are mostly interested in exploring
current data in order to allow
stakeholders to gain the freshest insights.
This definitely won't be possible if
the data being moved is already outdated.
A lot goes into ETL quality testing,
and it can be a tricky process,
but remembering these seven key elements is
a wonderful first step
toward creating high-quality pipelines.
Coming up, you're going to learn
even more about these checks and
other performance tests for ETL processes. Bye for now. 


## Seven elements of quality testing

In this part of the course, you have been learning about the importance of quality testing in your ETL system. This is the process of checking data for defects in order to prevent system failures. Ideally, your pipeline should have checkpoints built-in that identify any defects before they arrive in the target database system. These checkpoints ensure that the data coming in is already clean and useful! In this reading, you will be given a checklist for what your ETL quality testing should be taking into account. 

Checking for data quality involves ensuring the data is trustworthy before reaching its destination. When considering what checks you need to ensure the quality of your data as it moves through the pipeline, there are seven elements you should consider:

    Completeness: Does the data contain all of the desired components or measures?

    Consistency: Is the data compatible and in agreement across all systems?

    Conformity: Does the data fit the required destination format?

    Accuracy: Does the data conform to the actual entity being measured or described?

    Redundancy: Is only the necessary data being moved, transformed, and stored for use?

    Timeliness: Is the data current?

    Integrity: Is the data accurate, complete, consistent, and trustworthy? *

* _Integrity is influenced by the previously mentioned qualities. Quantitative validations, including checking for duplicates, the number of records, and the amounts listed, help ensure data’s integrity._

- Common issues

There are also some common issues you can protect against within your system to ensure the incoming data doesn’t cause errors or other large-scale problems in your database system:

    Check data mapping: Does the data from the source match the data in the target database?

    Check for inconsistencies: Are there inconsistencies between the source system and the target system?

    Check for inaccurate data: Is the data correct and does it reflect the actual entity being measured?

    Check for duplicate data: Does this data already exist within the target system?

To address these issues and ensure your data meets all seven elements of quality testing, you can build intermediate steps into your pipeline that check the loaded data against known parameters. For example, to ensure the timeliness of the data, you can add a checkpoint that determines if that data matches the current date; if the incoming data fails this check, there’s an issue upstream that needs to be flagged. Considering these checks in your design process will ensure your pipeline delivers quality data and needs less maintenance over time.

- Key takeaways

One of the great things about BI is that it gives us the tools to automate certain processes that help save time and resources during data analysis– building quality checks into your ETL pipeline system is one of the ways you can do this! Making sure you are already considering the completeness, consistency, conformity, accuracy, redundancy, integrity, and timeliness of the data as it moves from one system to another means you and your team don’t have to check the data manually later on.


## Monitor data quality with SQL

As you’ve learned, it is important to monitor data quality. By monitoring your data, you become aware of any problems that may occur within the ETL pipeline and data warehouse design. This can help you address problems as early as possible and avoid future problems.

In this reading, you’ll follow a fictional scenario where a BI engineer performs quality testing on their pipeline and suggests SQL queries that one could use for each step of testing.

- The scenario

At Francisco’s Electronics, an electronics manufacturing company, a BI engineer named Sage designed a data warehouse for analytics and reporting. After the ETL process design, Sage created a diagram of the schema.
The sales_warehouse database schema. The Sales table connects to the Products, Users, Locations, and Orders tables.

The diagram of the schema of the sales_warehouse database contains different symbols and connectors that represent two important pieces of information: the major tables within the system and the relationships among these tables.

The sales_warehouse database schema contains five tables:

    Sales 
    Products
    Users
    Locations
    Orders

These tables are connected via keys. The tables contain five to eight columns (or attributes) ranging in data type. The data types include varchar or char (or character), integer, decimal, date, text (or string), timestamp, and bit.

The foreign keys in the Sales table link to each of the other tables:

    The “product_id” foreign key links to the Products table
    The “user_id” foreign key links to the Users table
    The “order_id” foreign key links to the Orders table 
    The “shipping_address_id” and “billing_address_id” foreign keys link to the Locations table

After Sage made the sales_warehouse database, the development team made changes to the sales site. As a result, the original OLTP database changed. Now, Sage needs to ensure the ETL pipeline works properly and that the warehouse data matches the original OLTP database. 

Sage used the original OLTP schema from the store database to design the warehouse.
The original store database schema. The Sales table connects to the Products, Users, Locations, and Orders tables.

The store database schema also contains five tables—Sales, Products, Users, Locations, and Orders—which are connected via keys. The tables contain four to eight columns ranging in data type. The data types include varchar or char, integer, decimal, date, text, timestamp, bit, tinyint, and datetime.

Every table in the store database has an id field as a primary key. The database contains the following tables:

    The Sales table has price, quantity, and date columns. 
    - It references a user who made a sale (UserId), purchased a product (ProductId), and a related order (OrderId). 
    - Also, it references the Locations table for shipping and billing addresses (ShippingAddressId and BillingAddressId, respectively).

    The Users table has FirstName, LastName, Email, Password, and other user-related columns.

    The Locations table contains address information (Address1, Address2, City, State, and Postcode).

    The Products table has Name, Price, InventoryNumber, and Category of products.

    The Orders table has OrderNumber and purchase information (Subtotal, ShippingFee, Tax, Total, and Status).

- Using SQL to find problems

Sage compared the sales_warehouse database to the original store database to check for completeness, consistency, conformity, accuracy, redundancy, integrity, and timeliness. Sage ran SQL queries to examine the data and identify quality problems. Then Sage prepared the following table of lists, which include the types of quality issues found, the quality strategies that were violated, the SQL codes used to find the issues, and specific descriptions of the issues.

- Quality testing sales_warehouse

Tested quality  /  Quality strategy  /  SQL query  /  Sage’s Observation

1. Integrity: Is the data accurate, complete, consistent, and trustworthy?
	
        SELECT * 
        FROM Orders
	
_In the sales_warehouse database, the order with ID 7 has the incorrect total value._

2. Completeness: Does the data contain all of the desired components or measures?
	
        SELECT COUNT(*) 
        FROM Locations
	
_The Locations table of the sales_warehouse database has an extra address. In the store database there are 60 records, whereas the sales_warehouse database table has 61._

3. Consistency: Is the data compatible and in agreement across all systems?
	
        SELECT Phone 
        FROM Users
	
_Several users within the sales_warehouse database have phones without the "+" prefix._

4. Conformity: Does the data fit the required destination format?
	
        SELECT id, postcode 
        FROM sales_warehouse.Locations
	
_The location ZIP code for the record with ID 6 in the sales_warehouse database is 722434213, which is wrong. The United States postal code contains either five digits or five digits followed by a hyphen (dash) and another four digits (e.g., 12345-1234)._

- Quality testing store

Feature  /  Quality Strategy  /  SQL query  /  Sage’s Observation

1. Integrity: Is the data accurate, complete, consistent, and trustworthy?
	
        DESCRIBE Users

_Users.Status from the store database and Users.is_active from the sales_warehouse database seem to be related fields. However, it is not obvious how the Status column is transformed into the is_active boolean column. Is it possible that with a new status value, the ETL pipeline will fail?_

2. Consistency: Is the data compatible and in agreement across all systems?
	
        DESCRIBE Products
	
_Products.Inventory from the store database has the varchar type instead of the int(10) in the sales_warehouse database Products.inventory field. This can be a problem if there is a value with characters._

3. Accuracy: Does the data conform to the actual entity being measured or described?
	
        DESCRIBE Sales
	
_The data type of Sales.Date in the store database is different from its data type in sales_warehouse (date vs datetime). It might not be a problem if time is not important for the sales_warehouse database fact table._

4. Redundancy: Is only the necessary data being moved, transformed, and stored for use?
	
        DESCRIBE Sales
	
_The table Sales from the sales_warehouse database has a unique index constraint on OrderId, ProductId, UserId columns. It can be added to the warehouse schema._

- Key takeaways:

Testing data quality is an essential skill of a BI professional that ensures good analytics and reporting. Just as Sage does in this example, you can use SQL commands to examine BI databases and find potential problems. The sooner you know the problems in your system, the sooner you can fix them and improve your data quality.


## Mana: Quality data is useful data

My name is Mana and I am
a Senior Technical Data Program Manager at Google.
What that means is that I work
with business partners and I help
create tools that help enable them
to make better decisions with data.
I'm a big data nerd,
so I love playing around with data and getting to build
cool stuff that makes people's jobs a lot easier.
There's a common saying that in
the absence of data you have dirt.
I like to take that a step further.
I like to say in the absence of good data, you have dirt.
Quality testing is all about
how do you make sure that you have good data.
Good data can mean a number of different things.
Oftentimes, it means accurate data.
How do you ensure that the numbers you are producing
are correct and they're representative of the truth.
It can also mean relevant data.
It can also mean representative data.
It can also mean quick data at your fingertips.
The process of quality control is making sure that
the tools that you're building with
respect to data are accurate,
helpful, relevant, and timely.
There are many times across the life-cycle of
building a BI product in
which quality testing comes into play.
If you think of the very early stages where maybe
someone is trying to extract data from logs,
you're going to want to make sure that the data
that you're extracting is accurate.
It's the same data that's coming in through the logs,
the same data that's being spit out
from the data mart maybe that I'm creating.
It's the same idea through
your ETL processes where ETL
means extract, transform and load.
As you're grabbing the data, you're transforming it,
you're massaging it, and you're
creating relevancy with that data.
You want to make sure that the data you
got in is the same data you're spitting out.
I remember when I was a young professional,
I was always imagining that
one day I would land at a company that was
data nirvana and all of their data would be so
clean and so perfect and it was just magical,
I could just query it with no worries in the world.
The truth is that nirvana does not exist anywhere.
Data always has issues.
There are always bugs that come up.
Even the data that you were looking at today might
be different than the data that you look at tomorrow.
Embedding quality testing,
not only as a one-off,
but as a regular process
in your pipelines or whatever that you're
building is of incredible importance
because bugs are just bound to happen.
There are a couple of things that I
wish I knew when I was starting out.
I wish that I had fully been able to
recognize how many skills I had in
this department that came from other parts of my life and
weren't the traditional means of BI skills,
and with that, having more confidence in myself
because I came in with
really fantastic storytelling skills
that I was really able to hone in on.
Even though I wasn't a software engineer,
I have a lot of experience coding and I knew a lot
of best practices that I was able to put in place.
I would say that if there are areas that
you feel like you're maybe not the strongest in,
that if you stay curious and you
stay open and you stay humble,
and you find folks that are
really great at those and you ask them,
hey, how do you do that?
Know that you can learn and
you can grow in those capacities,
and you can become continuously well-rounded.
It's very normal for us as humans to
have our strengths and our growth areas.
But being successful is not having them innately.
It's having the ability to constantly
evolve better yourself and not become the expert,
but just become better than you were yesterday. 



# DATA SCHEMA VALIDATION

## Conformity from source to destination

You're learning a lot about the importance
of quality testing and ETL,
and you now know that
a key part of the process is checking for
conformity or whether the data
fits the required destination format.
To ensure conformity,
from source to destination,
BI professionals have three very effective tools;
schema validation, data dictionaries and data lineages.
In this video, we'll examine how they can
help you establish consistent data governance.
First, schema validation is a process to ensure that
the source system data schema
matches the target database data schema.
As you're learning, if the schemas don't align,
this can cause system failures
that are very difficult to fix.
Building schema validation into your workflow,
is important to prevent these issues.
Database tools offer
various schema validation options that can be used
to check incoming data against
the destination schema requirements.
For example, you could dictate that
a certain column contains only numerical data.
Then if you try to enter
something in that column that doesn't conform,
the system will flag the error.
Or in a relational database,
you could specify that an ID number
must be a unique field.
That means the same ID can't be
added if it matches an existing entry.
This prevents redundancies in the data.
With these properties and action,
if the data doesn't conform and throws an error,
you'll be alerted, or if it meets the requirements,
you'll know it's valid and safe to load.
Schema validation properties should ensure three things.
The keys are still valid after transformation.
The table relationships have been preserved,
and the conventions are consistent across the database.
Let's start with the keys.
As you've been learning, relational databases use
primary and foreign keys to
build relationships among tables.
These keys should continue to function
after you've moved data from one system into another.
For example, if your source system
uses customer_id as a key,
then that needs to be valid
and the target schema as well.
This is related to the next
property of schema validation,
making sure the table relationships have been preserved.
When taking in data from a source system,
it's important that these keys remain valid
in the target system so the relationships can
still be used to connect tables or that
they are transformed to match the target schema.
For example, if the customer_id key
doesn't apply to our target system
then all of the tables that used it as
a primary or foreign key are disconnected.
If there are relationships between tables have
been broken and while data is being moved,
then data becomes hard to access and use,
and that's the whole reason we
moved it to our target system.
Finally, you want to ensure that
the conventions are consistent
with the target database's schema.
Sometimes data from outside sources uses
different conventions for naming columns and tables.
For example, you could have a source system that uses
employee ID as one word to identify that field,
but the target database might use employee_id.
You'll need to ensure these are consistent so you don't
get errors when trying to pull data for analysis.
In addition to the properties themselves,
there are some other documentation tools
that support data schema validation;
data dictionaries and data lineages.
A data dictionary is a collection of
information that describes the content,
format and structure of data objects within a database,
as well as their relationships.
You might also hear this referred
to as a metadata repository.
You may know that metadata is data about data.
This is a very important concept in BI,
so if you'd like to review some of the lessons about
metadata from the Google Data Analytics certificate,
go ahead and do that now.
In the case of data dictionaries,
these represent metadata because
they're basically using one type of data,
metadata, to define the use
and origin of another piece of data.
There are several reasons you might want to
create a data dictionary for your team.
For one thing, it helps avoid
inconsistencies throughout a project.
In addition, it enables you to
define any conventions that
other team members need to know in order
to create more alignment across teams.
Best of all, it makes the data easier to work with.
Now, let's explore data lineages.
Data lineage describes a process
of identifying the origin of data,
where it has moved throughout the system,
and how it has transformed over time.
This is useful because if you do get an error,
you can track the lineage of that piece of data,
and understand what happened
along the way to cause the problem.
Then, you can put standards in
place to avoid the same issue in the future.
Using schema validation, data dictionaries,
and data lineages really helps BI professionals promote
consistency as data is
moved from the source to destination.
This means all users can be
confident in the BI solutions being created.
We'll keep exploring these concepts soon.


## Sample data dictionary and data lineage

As you have been learning in this course, business intelligence professionals have three primary tools to help them ensure conformity from source to destination: schema validation, data dictionaries, and data lineages. In this reading, you’re going to explore some examples of data dictionaries and lineages to get a better understanding of how these items work.

- Data dictionaries

A data dictionary is a collection of information that describes the content, format, and structure of data objects within a database, as well as their relationships. This can also be referred to as a metadata repository because data dictionaries use metadata to define the use and origin of other pieces of data. Here’s an example of a PRODUCT TABLE that exists within a sales database:

        Item_ID    Price    Department    Number_of_Sales    Number_in_Stock    Seasonal
        47257      $33.00   Gardening       744                598                Yes
        39496      $82.00   Home Decor      383                729                Yes
        73302      $56.00   Furniture       874                193                No
        16507      $100.00  Home Office     310                559                Yes
        1232       $125.00  Party Supplies  351                517                No
        3412       $45.00   Gardening       901                942                No
        54228      $60.00   Party Supplies  139                520                No
        66415      $38.00   Home Decor      615                433                Yes
        78736      $12.00   Grocery         739                648                No
        34369      $28.00   Gardening       555                389                Yes

This table is actually the final target table for data gathered from multiple sources. It's important to ensure consistency from the sources to the destination because this data is coming from different places within the system. This is where the data dictionary comes in:

- Data dictionary

_Name: Definition - Data Type_

    Item_ID: ID number assigned to all product items in-store - Integer
    
    Price: Current price of product item - Integer
    
    Department: Which department the product item belongs to - Character
    
    Number_of_Sales: The current number of product items sold - Integer
    
    Number_in_Stock: The current number of product items in stock - Integer
    
    Seasonal: Whether or not the product item is only seasonally available - Boolean

You can use the properties outlined in the dictionary to compare incoming data to the destination table. If any data objects don’t match the entries in the dictionary, then the data validation will flag the error before the incorrect data is ingested.

For example, if incoming data that is being delivered to the Department column contains numerical data, you can quickly identify that there has been an error before it gets delivered because the data dictionary states Department data should be character-type.

- Data lineages

A data lineage describes the process of identifying the origin of data, where it has moved throughout the system, and how it has transformed over time. This can be really helpful for BI professionals, because when they do encounter an error, they can actually track it to the source using the lineage. Then, they can implement checks to prevent the same issue from occuring again.

For example, imagine your system flagged an error with some incoming data about the number of sales for a particular item. It can be hard to find where this error occurred if you don’t know the lineage of that particular piece of data– but by following that data’s path through your system, you can figure out where to build a check.

< An illustration of data moving through a system >

By tracking the sales data through its life cycle in the system, you find that there was an issue with the original database it came from and that data needs to be transformed before it’s ingested into later tables.

- Key takeaways

Tools such as data dictionaries and data lineages are useful for preventing inconsistencies as data is moved from source systems to its final destination. It is important that users accessing and using that data can be confident that it is correct and consistent. These tools actively track and validate data throughout its journey, ensuring it's reliable for analysis and decision-making. This is key for building trustworthy reports and dashboards as a BI professional!


## Check your schema

One of the best ways to learn is through a case study.
When you witness how something
happened at an actual organization,
it really brings ideas and concepts to life.
In this video, we're going to check out
schema governance in action at an educational non-profit.
In this scenario, decision-makers at
the non-profit are interested in
measuring educational outcomes in their community.
In order to do this, they are ingesting data from
school databases in order to evaluate learning goals,
national education statistics, and students surveys.
Because they're pulling data from
multiple sources into their own database system,
it's important that they maintain consistency across
all the data to prevent
errors and avoid losing important information.
Luckily, this organization already has
a data dictionary and lineage in
place to establish the necessary standards.
Let's check out an example of
a column from the student information table.
This table has five columns.
Student ID, school system,
school, age, and grade point average.
Each column in this table has been recorded in
the data dictionary to
specify what information it contains,
so we can go to the data dictionary entry for
the school system column to
double-check the standards for this table.
As a refresher, a data dictionary is
a collection of information that describes the content,
format, and structure of
data objects within a database and their relationships.
This dictionary records four specific properties,
the name of the column, its definition,
the datatype, and possible values.
The dictionary entry for age lets us know
the data objects in this column
contain information about a student's age.
It also tells us that this is integer type data.
We can use these properties to compare
incoming data to the destination table.
If any data objects aren't integer type data,
then the schema validation will flag the error
before the incorrect data is
ingested into the destination.
What happens when a data object
fails to schema validation process?
We can actually use the data lineage
to trace the journey of this piece of
data and find out where in
the process we might want to add a quality check.
Again, a data lineage
includes information about the data's origin,
where it is moved throughout the system,
and how it has transformed over time.
During the schema validation process,
this piece of data through an error because it
isn't currently cast as integer type.
When we check the data lineage,
we can track this object's movement through our system.
This data started in an individual schools database
before being read into the school systems database.
The individual schools data was ingested by
our pipeline along with data from other school systems,
and then organize and transformed
during the movement process.
Apparently, when this data was
input in the schools original database,
it wasn't type casted correctly.
We can confirm that by checking
its datatype throughout the lineage.
Lineage also includes all the transformations
that this data has undergone so far.
Also, we might at this point
notice that type casting isn't built into
our transformation process during
quality checks. That's great news.
Now we know that that's
a process we should incorporate into
the pipeline before data is
read into the destination table.
In this case, age data objects should be integer type,
and that's how schema governance and validation can
help improve systems and prevent errors.
There are other tests that should be applied
to a pipeline to make sure it's functioning correctly,
which we'll learn more about soon.
But now you have a better
understanding of how to validate
the schema and keep improving your pipeline processes. 


## Schema-validation checklist

In this course, you have been learning about the tools business intelligence professionals use to ensure conformity from source to destination: schema validation, data dictionaries, and data lineages. In another reading, you already had the opportunity to explore data dictionaries and lineages. In this reading, you are going to get a schema validation checklist you can use to guide your own validation process.

Schema validation is a process used to ensure that the source system data schema matches the target database data schema. This is important because if the schemas don’t align, it can cause system failures that are hard to fix. Building schema validation into your workflow is important to prevent these issues.

- Common issues for schema validation:

1. The keys are still valid: Primary and foreign keys build relationships between tables in relational databases. These keys should continue to function after you have moved data from one system into another.

2. The table relationships have been preserved: The keys help preserve the relationships used to connect the tables so that keys can still be used to connect tables. It’s important to make sure that these relationships are preserved or that they are transformed to match the target schema.

3. The conventions are consistent: The conventions for incoming data must be consistent with the target database’s schema. Data from outside sources might use different conventions for naming columns in tables– it’s important to align these before they’re added to the target system.

- Using data dictionaries and lineages:

You’ve already learned quite a bit about data dictionaries and lineages. As a refresher, a data dictionary is a collection of information that describes the content, format, and structure of data objects within a database, as well as their relationships. And a data lineage is the process of identifying the origin of data, where it has moved throughout the system, and how it has transformed over time. These tools are useful because they can help you identify what standards incoming data should adhere to and track down any errors to the source.

- Key takeaways:

Schema validation is a useful check for ensuring that the data moving from source systems to your target database is consistent and won’t cause any errors. Building in checks to make sure that the keys are still valid, the table relationships have been preserved, and the conventions are consistent before data is delivered will save you time and energy trying to fix these errors later on.



# BUSINESS RULES & PERFORMANCE TESTING

## Verify business rules

So far, we've learned a lot about database performance, quality testing and
schema validation and how these checks ensure the database and
pipeline system continue to work as expected.
Now we're going to explore another important check, making sure
that the systems and processes you have created actually meet business needs.
This is essential for
ensuring that those systems continue to be relevant to your stakeholders.
To do this by professionals verify business rules.
In BI,
A business rule is a statement that creates a restriction on specific parts of
a database.
For example, a shipping database might impose a business rule that states
shipping dates can't come before order dates.
This prevents order dates and shipping dates from being mixed up and
causing errors within this system.
Business rules are created according to the way a particular organization
uses its data in a previous video, we discovered how important it can be to
observe how a business uses data before building up database system.
Understanding the actual needs, guides, design.
And this is true for business rules too.
The business rules you create will affect a lot of the databases,
design what data is collected and stored, how relationships are defined,
what kind of information the database provides and the security of the data.
This helps ensure the database is performing as intended.
Business rules are different in every organization because the way
organizations interact with their data is always different.
Plus business rules are also always changing.
Which is why keeping a record of what rules exist and why is critical.
Here's another example: consider a library database.
The primary need of the users who are librarians in this
case is to check out books and maintain information about patrons. Because of this,
there are a few business rules this library might impose on the database to
regulate the system.
One rule could be that library patrons cannot check out more than five books
at a time.
The database won't let a user check out a sixth book. Or the database could have a rule
that the same book cannot be checked out by two people at the same time.
If someone tries, the librarians would be alerted that there's a redundancy.
Another business rule could be that specific information must be entered
into the system for a new book to be added to the library inventory.
Basically verification involves ensuring that data imported into the target
database complies with business rules on top of that.
These rules are important pieces of knowledge that help a BI professional
understand how a business and
its processes function.
This helps the BI
professional become a subject matter
expert and trusted advisor.
As you're probably noticing this process is very similar to schema validation.
In schema validation,
you take the target database's schema and compare incoming data to it.
Data that fails
this check is not ingested into the destination database.
Similarly, you will compare incoming data to the business rules before loading it
into the database. In our library example, if a patron puts in a request for
a book but they already have more than five books from the library, then this
incoming data doesn't comply with the preset business rule, and it prevents them
from checking out the book. And that's the basics about verifying business rules.
These checks are important because they ensure that databases do their jobs as
intended. And because business rules are so integral to the way databases function,
verifying that they're working correctly is very important.
Coming up, you'll get a chance to explore business rules in more detail. 


## Business rules

As you have been learning, a business rule is a statement that creates a restriction on specific parts of a database. These rules are developed according to the way an organization uses data. Also, the rules create efficiencies, allow for important checks and balances, and also sometimes exemplify the values of a business in action.  For instance, if a company values cross-functional collaboration, there may be rules about at least 2 representatives from two teams checking off completion on some data set. They affect what data is collected and stored, how relationships are defined, what kind of information the database provides, and the security of the data. In this reading, you will learn more about the development of business rules and see an example of business rules being implemented in a database system.

- Imposing business rules

Business rules are highly dependent on the organization and their data needs. This means business rules are different for every organization. This is one of the reasons why verifying business rules is so important; these checks help ensure that the database is actually doing the job you need it to do. But before you can verify business rules, you have to implement them.

For example, let’s say the company you work for has a database that manages purchase order requests entered by employees. Purchase orders over $1,000 dollars need manager approval. In order to automate this process, you can impose a ruleset on the database that automatically delivers requests over $1,000 to a reporting table pending manager approval. Other business rules that may apply in this example are: prices must be numeric values (data type should be integer); or for a request to exist, a reason is mandatory (table field may not be null).

< Flow chart represents the three business rules: product order requests, requests pending approval and approved product order >

In order to fulfill this business requirement, there are three rules at play in this system:

1. Order requests under $1,000 are automatically delivered to the approved product order requests table
2. Requests over $1,000 are automatically delivered to the requests pending approval table
3. Approved requests are automatically delivered to the approved product order requests table

These rules inherently affect the shape of this database system to cater to the needs of this particular organization.

- Verifying business rules

Once the business rules have been implemented, it’s important to continue to verify that they are functioning correctly and that data being imported into the target systems follows these rules. These checks are important because they test that the system is doing the job it needs to, which in this case is delivering product order requests that need approval to the right stakeholders. 

- Key takeaways

Business rules determine what data is collected and stored, how relationships are defined, what kind of information the database provides, and the security of the data. These rules heavily influence how a database is designed and how it functions after it has been set up. Understanding business rules and why they are important is useful as a BI professional because this can help you understand how existing database systems are functioning, design new systems according to business needs, and maintain them to be useful in the future.


## Database performance testing in an ETL context

In previous lessons, you learned about database optimization as part of the database building process. But it’s also an important consideration when it comes to ensuring your ETL and pipeline processes are functioning properly. In this reading, you are going to return to database performance testing in a new context: ETL processes.

- How database performance affects your pipeline

Database performance is the rate that a database system is able to provide information to users. Optimizing how quickly the database can perform tasks for users helps your team get what they need from the system and draw insights from the data that much faster.

Your database systems are a key part of your ETL pipeline– these include where the data in your pipeline comes from and where it goes. The ETL or pipeline is a user itself, making requests of the database that it has to fulfill while managing the load of other users and transactions. So database performance is not just key to making sure the database itself can manage your organization’s needs– it’s also important for the automated BI tools you set up to interact with the database.

- Key factors in performance testing

Earlier, you learned about some database performance considerations you can check for when a database starts slowing down. Here is a quick checklist of those considerations:

    Queries need to be optimized
    The database needs to be fully indexed
    Data should be defragmented
    There must be enough CPU and memory for the system to process requests

You also learned about the five factors of database performance: workload, throughput, resources, optimization, and contention. These factors all influence how well a database is performing, and it can be part of a BI professional’s job to monitor these factors and make improvements to the system as needed.

These general performance tests are really important– that’s how you know your database can handle data requests for your organization without any problems! But when it comes to database performance testing while considering your ETL process, there is another important check you should make: testing the table, column, row counts, and Query Execution Plan.

Testing the row and table counts allows you to make sure that the data count matches between the target and source databases. If there are any mismatches, that could mean that there is a potential bug within the ETL system. A bug in the system could cause crashes or errors in the data, so checking the number of tables, columns, and rows of the data in the destination database against the source data can be a useful way to prevent that.

- Key takeaways

As a BI professional, you need to know that your database can meet your organization’s needs. Performance testing is a key part of the process. Not only is performance testing useful during database building itself, but it’s also important for ensuring that your pipelines are working properly as well. Remembering to include performance testing as a way to check your pipelines will help you maintain the automated processes that make data accessible to users!


## Defend against known issues

In this reading, you’ll learn about a defensive check applied to a data pipeline. Defensive checks help you prevent problems in your data pipeline. They are similar to performance checks but focus on other kinds of problems. The following scenario will provide an example of how you can implement different kinds of defensive checks on a data pipeline.

- Scenario

Arsha, a Business Intelligence Analyst at a telecommunications company, built a data pipeline that merges data from six sources into a single database. While building her pipeline, she incorporated several defensive checks that ensured that the data was moved and transformed properly.

Her data pipeline used the following source systems:

    Customer details
    Mobile contracts
    Internet and cable contracts
    Device tracking and enablement
    Billing
    Accounting

All of these datasets had to be harmonized and merged into one target system for business intelligence analytics. This process required several layers of data harmonization, validation, reconciliation, and error handling.

- Pipeline layers

Pipelines can have many different stages of processing. These stages, or layers, help ensure that the data is collected, aggregated, transformed, and staged in the most effective and efficient way. For example, it’s important to make sure you have all the data you need in one place before you start cleaning it to ensure that you don’t miss anything. There are usually four layers to this process: staging, harmonization, validation, and reconciliation. After these four layers, the data is brought into its target database and an error handling report summarizes each step of the process.

< Diagram of the pipeline layers. Sources feed into each layer before entering the target table or error handling report. >

- Staging layer

First, the original data is brought from the source systems and stored in the staging layer. In this layer, Arsha ran the following defensive checks:

    Compared the number of records received and stored
    Compared rows to identify if extra records were created or records were lost
    Checked important fields, such as amounts, dates, and IDs

Arsha moved the mismatched records to the error handling report. She included each unconverted source record, the date and time of its first processing, its last retry date and time, the layer where the error happened, and a message describing the error. By collecting these records, Arsha was able to find and fix the origin of the problems. She marked all of the records that moved to the next layer as “processed.”

- Harmonization layer

The harmonization layer is where data normalization routines and record enrichment are performed. This ensures that data formatting is consistent across all the sources. To harmonize the data, Arsha ran the following defensive checks:

    Standardized the date format
    Standardized the currency
    Standardized uppercase and lowercase stylization
    Formatted IDs with leading zeros
    Split date values to store the year, month, and day in separate columns
    Applied conversion and priority rules from the source systems

When a record couldn’t be harmonized, she moved it to Error Handling. She marked all of the records that moved to the next layer as “processed.”

- Validations layer

The validations layer is where business rules are validated. As a reminder, a business rule is a statement that creates a restriction on specific parts of a database. These rules are developed according to the way an organization uses data. Arsha ran the following defensive checks:

    Ensured that values in the “department” column were not null, since “department” is a crucial dimension
    Ensured that values in the “service type” column were within the authorized values to be processed
    Ensured that each billing record corresponded to a valid processed contract

Again, when a record couldn’t be validated, she moved it to error handling. She marked all the records that moved to the next layer as “processed.”

- Reconciliation layer

The reconciliation layer is where duplicate or illegitimate records are found. Here, Arsha ran defensive checks to find the following types of records:

    Slow-changing dimensions
    Historic records
    Aggregations

As with the previous layers, Arsha moved the records that didn't pass the reconciliation rules to Error Handling. After this round of defensive checks, she brought the processed records into the BI and Analytics database (OLAP).

- Error handling reporting and analysis

After completing the pipeline and running the defensive checks, Arsha made an error handling report to summarize the process. The report listed the number of records from the source systems, as well as how many records were marked as errors or ignored in each layer. The end of the report listed the final number of processed records.

< Summary of number of records from source and how many were processed, marked as errors, or ignored in each pipeline layer. >

- Key takeaways

Defensive checks are what ensure that a data pipeline properly handles its data. Defensive checks are an essential part of preserving data integrity. Once the staging, harmonization, validations, and reconciliation layers have been checked, the data brought into the target database is ready to be used in a visualization.


## Burak: Evolving technology

My name is Burak.
I'm a BI Engineer in Google.
What a BI Engineer does is actually collecting,
storing, and analyzing data
with a lot of infrastructure involved.
I moved to States five years ago as a fresh immigrant.
It was very difficult to get the first job for me.
Even though I have a degree,
I still needed to a lot of training to get
ready for the domestic needs of the market.
I started teaching myself what a BI engineer does?
What are the essential
technical skills that I need to learn?
I did a lot of online research.
I found a lot of free stuff,
I found a couple of
paid subscriptions and I started learning
all these technical skills that
I need to learn to get my first job.
BI technology evolved a lot over the last 10 years.
I can say spreadsheets very in 10 years ago,
but nobody is a specialist
anymore in terms of data analysis.
I mean, it's still being used for quick analysis,
but now everything has evolved into Cloud,
technologies, more sophisticated languages,
more powerful visual tools to help everyone.
Personally, I have to adapt,
changing new environments and
new languages and new infrastructures.
In order to keep up with the technology,
you actually need to do a little bit research and
understand how the industry is actually evolving.
There are lots of online resources or
web pages or newsletters that you
can follow about the latest industrial trends.
But the essentials, they never change.
The foundation of the BI engineering is the same.
If you learn a SQL language,
whatever organization you work
for is going to be a different SQL language,
is going to be different dialects.
You still need to catch up with,
but the amount of time that you need to learn is going to
be drastically less than
the amount of time you first start.
Because there's going to be transferable skills.
My number one piece advice will be dedication.
If you really love working with data and
if you would like to work in this field,
dedication is one of
the key requirements because there is
a lot of technical skills that you
need to learn and it needs time.
Therefore, I recommend to identify
which area of BI engineering
that you actually want to focus on,
because there are several parts that you can work.
You can build infrastructures,
or you can design systems,
or you can analyze data,
or you can do some visualization tools.
Depending on which area you would like to focus on,
the technical skills you need to learn will vary. 


## Case study: FeatureBase, Part 2: Alternative solutions to pipeline systems

This case study with FeatureBase will focus on the Analyze stage of the BI process, where you examine relationships in the data, draw conclusions, make predictions, and drive informed decision-making. This follows an earlier case study, where you explored the Capture phase of FeatureBase’s project. In a follow-up case study, you’ll learn about how FeatureBase addressed the Monitor stages of this project to solve their business problem. Like the previous FeatureBase case study, you’ll consider the problem, process, and solution for this stage of the project.

In a previous reading, you were introduced to FeatureBase, the OLAP database company. For a quick refresher, you can review part one of this case study. Their core technology, FeatureBase, is the first OLAP database built entirely on bitmaps that power real-time analytics and machine learning applications by simultaneously executing low latency, high throughput, and highly concurrent workloads. Last time, you learned about a business problem the FeatureBase team was facing: they realized that customers were falling off during the sales cycle, but that their data collection didn’t have the necessary measurements to investigate when and why this was happening. The first step to addressing this issue was collaborating across sales, marketing, and leadership teams to determine what data they needed to understand when customers were falling off. Then, they could use that insight to investigate and address those issues for future sales. In this reading, you’re going to focus on the database tools FeatureBase uses to collect data for monitoring and reporting. 

- Feature-oriented databases

Throughout this program, you have been learning about different database technologies that use pipeline systems to ingest, transform, and deliver data to target databases. This setup is fairly common across many different organizations, and you will often work with pipelines as a BI professional. However, there are also other types of database systems that use different technology to make data accessible and useful to users. 

FeatureBase is one example of an alternative solution to traditional databases– it is built on top of bitmaps, which is a format that stores data as raw features. To build predicting models, the AI depends on the feature-oriented database (and not the other way around) to find patterns which can be used to guide decision making. These models are fed measurable data points, or features, that help it learn how to parse the data more effectively over time. Feature-oriented databases provide an alternate approach to data prep by automating the feature extraction as the first step. The feature-oriented approach enables real-time analytics and AI initiatives because the data or "features" are already in a model-ready data format that is instantly accessible and reusable across the organization, without the need to re-copy or re-pre-process. 

Here’s an example of this system: imagine you were trying to predict a type of animal based on traits. Humans would have a list of traits they might think about: wings, snouts, or the number of legs, for example. But these traits aren’t actionable like that– but if they’re converted into features like “has_wings” or “has_4_legs” with yes or no values coded as 1 or 0,  they can be fed into a model and processed more quickly. This is why FeatureBase is built on bitmaps; the arrays of 1s and 0s are easily actionable by machines and models.

< A feature table with four features organized in columns: animal_id, is_snake, is_poisionous, and send_alert. >

- Fine-tuning features

In the last reading, you followed along as FeatureBase leadership considered how to approach their ultimate question: Why are customers dropping off during the sales cycle?

At that point in this project’s cycle, the team didn’t have metrics built into their system to find out when customers weren’t completing the sales process, which was key to investigating why customers were dropping off. Having determined what their system was lacking, the team encoded these new features into the collection process– they recreated their original sales funnel with new attributes about customers at every stage of the sales cycle. These new features were fed into their database model, which began training to identify patterns, allowing them to immediately draw insights from their pool of data.  

One of the attributes they added to the data collection process tracked exactly when customers were dropping off.  They discovered that most customers who didn’t complete the sale dropped off during the technical validation stage. This is the point at which the FeatureBase team would set up FeatureBase within the customer’s system so they can try the product for themselves. The team realized that this was the critical stage they needed to investigate more. They theorized that customers weren’t leaving the technical validation stage confident about their ability to adopt this new technology. They also wondered if customers were having concerns about the reliability and stability of the product since FeatureBase would replace their current, still-functioning database system. To understand this better, they would need to explore the customer data gathered at this stage in their dashboard. 

- The next step

As a BI professional, you might find yourself working with a variety of database technologies connected with pipeline systems like more traditional row based technologies and newer alternatives such as FeatureBase. Understanding your tools and how they operate will help you focus on what’s most important–empowering your team with access to the answers they need. As they continued investigating their problem, the FeatureBase team found that most customers who did not complete the sales process were falling off in the technical validation stage. 

This is the point at which FeatureBase was being implemented in the customer’s data environment to determine if it was actually functional for them. This is how the FeatureBase team can showcase FeatureBase’s utility and provide proof that it is a workable solution for a customer’s needs.  

The team theorized that, while many customers loved the capabilities of the service, they had some anxieties about how adoptable it would be for their organization and how reliable it would be. But before the team can confirm this theory or make any decisions based on this potential answer, they would need to be able to explore dashboard reports and investigate their metrics deeply. Which is what you will focus on when you return to this case study next time!



# REVIEW: OPTIMIZE ETL PROCESSES

## Wrap-Up

As BI professional, your job doesn't end once you've built the database systems and
pipeline tools for your organization.
It's also important that you ensure they continue to work as intended and
handle potential errors before they become problems
in order to address those ongoing needs.
You've been learning a lot.
First, you explored the importance of quality testing in an ETL system.
This involved checking incoming data for completeness, consistency,
conformity, accuracy, redundancy, integrity, and timeliness.
You also investigated schema governance and
how schema validation can prevent incoming data from causing errors in the system by
making sure it conforms to the scheme of properties of the destination database.
After that, you discovered why verifying business rules is an important step in
optimization because it ensures that the data coming in meets the business
needs of the organization using it.
Maintaining the storage systems that users interact with is an important part
of ensuring that your system is meeting the business's needs.
This is why database optimization is so important, but
it's just as important to ensure that the systems that move data from place to
place are as efficient as possible.
And that's where optimizing pipelines and ETL systems comes in.
Coming up, you have another assessment.
I know you can do this and just as a reminder,
you can review any of the material as you get ready as well as the latest glossary.
So feel free to revisit any videos or
readings to get a refresher before the assessment.
After that, you'll have the chance to put everything you've been learning into
practice by developing BI tools and processes yourself.
You're making excellent progress toward a career in BI. 


## Glossary

Accuracy: An element of quality testing used to confirm that data conforms to the actual entity being measured or described

Business rule: A statement that creates a restriction on specific parts of a database

Completeness: An element of quality testing used to confirm that data contains all desired components or measures

Conformity: An element of quality testing used to confirm that data fits the required destination format

Consistency: An element of quality testing used to confirm that data is compatible and in agreement across all systems

Data dictionary: A collection of information that describes the content, format, and structure of data objects within a database, as well as their relationships

Data lineage: The process of identifying the origin of data, where it has moved throughout the system, and how it has transformed over time

Data mapping: The process of matching fields from one data source to another

Integrity: An element of quality testing used to confirm that data is accurate, complete, consistent, and trustworthy throughout its life cycle

Quality testing: The process of checking data for defects in order to prevent system failures; it involves the seven validation elements of completeness, consistency, conformity, accuracy, redundancy, integrity, and timeliness

Redundancy: An element of quality testing used to confirm that no more data than necessary is moved, transformed, or stored

Schema validation: A process to ensure that the source system data schema matches the target database data schema

Timeliness: An element of quality testing used to confirm that data is current



# REVIEW: DATA ANALYTICS CONTENT

## Data integrity

Welcome back.
In this video, we're going to discuss data integrity and
some risk you might run into as a data analyst.
A strong analysis depends on the integrity of the data.
If the data you're using is compromised in any way,
your analysis won't be as strong as it should be.
Data integrity is the accuracy, completeness, consistency and
trustworthiness of data throughout its life cycle.
That might sound like a lot of qualities for the data to live up to.
But trust me, it's worth it to check for
them all before proceeding with your analysis.
Otherwise your analysis could be wrong, not because you did something wrong,
but because the data you were working with was wrong to begin with.
When data integrity is low, it can cause anything from the loss of a single
pixel in an image to an incorrect medical decision.
In some cases, one missing piece can make all of your data useless.
Data integrity can be compromised in lots of different ways.
There's a chance data can be compromised every time it's replicated,
transferred or manipulated in any way.
Data replication is the process of storing data in multiple locations.
If you're replicating data at different times in different places,
there's a chance your data will be out of sync.
This data lacks integrity because different people might not be using
the same data for their findings, which can cause inconsistencies.
There's also the issue of data transfer, which is the process of copying
data from a storage device to memory or from one computer to another.
If your data transfer is interrupted, you might end up with an incomplete data set,
which might not be useful for your needs.
The data manipulation process involves changing the data to make it
more organized and easier to read.
Data manipulation is meant to make the data analysis process more efficient, but
an error during the process can compromise that efficiency.
Finally, data can also be compromised through human error, viruses,
malware, hacking and system failures, which can all lead to even more headaches.
I'll stop there.
That's enough potentially bad news to digest.
Let's move on to some potentially good news.
And a lot of companies, the data warehouse or
data engineering team takes care of ensuring data integrity.
Coming up, we'll learn about checking data integrity as a data analyst.
But rest assured someone else will usually have your back too.
After you found out what kind of data you're working with, it's important to
double check that your data is complete and valid before analysis.
This will help ensure that your analysis and eventual conclusions are accurate.
Checking data integrity is a vital step in processing your data to get it ready for
analysis, whether you or someone else that your company is doing it.
Coming up, you'll learn even more about data integrity.
See you soon. 


## Metadata

Now that you understand the different ways
to organize data in a database,
let's talk about how you can describe that data.
In this video, we'll start exploring metadata,
which is a very important aspect of database management.
Metadata is an abstract concept though.
Let's kick things off with a simple, everyday example.
Did you know that every time
a photo is taken with a smartphone,
data is automatically collected
and stored within that photo?
Take a look. Choose any photo on your computer.
Here's a cute shot of my friend's dogs, Rudy and Matilda.
On your photo, right-click on "Get Info" or "Properties."
This will give you the photo's metadata,
which may tell you the type of file it is,
the date and time it was taken,
the geo-location or where it was taken,
what kind of device was used to
take the photo, and much more.
Pretty amazing, right?
Here's another example.
Every time you send or receive an email,
metadata is sent right along with that message.
You can find it by clicking on "Show
Original" or "View Message Details."
An email message's metadata includes its subject,
who it's from, who it's to,
and the date and time it was sent.
The metadata even knows how quickly it
was delivered after the sender pressed "Send."
Metadata is information that's used to describe
the data that's contained in
something like a photo or an email.
Keep in mind that metadata is not the data itself.
Instead, it's data about the data.
In data analytics, metadata helps data analysts
interpret the contents of the data within a database.
That's why metadata is so
important when working with databases.
It tells an analyst what the data is all about.
That makes it possible to put the data to work,
solving problems, and making data-driven decisions.
As a data analyst,
there are three common types of
metadata that you'll come across
: descriptive, structural, and administrative.
Descriptive metadata is metadata
that describes a piece of
data and can be used to
identify it at a later point in time.
For instance, the descriptive metadata of a book
in a library would include the code you see on its spine,
known as a unique International Standard Book Number,
also called the ISBN.
It would also include the book's author and title.
Next is structural metadata,
which is metadata that indicates how a piece of data is
organized and whether it's part of
one or more than one data collection.
Let's head back to the library.
An example of structural data would be how
the pages of a book are put
together to create different chapters.
It's important to note that structural metadata
also keeps track of the relationship between two things.
For example, it can show us that the digital document of
a book manuscript was actually
the original version of a now printed book.
Finally, we have administrative metadata.
Administrative metadata is metadata that
indicates the technical source of a digital asset.
When we looked at the metadata inside the photo,
that was administrative metadata.
It showed you the type of file it was,
the date and time it was taken, and much more.
Here's one final thought to help you understand metadata.
If you're on your way to the library to pick out a book,
you could research a book's title,
author, length, a number of chapters.
That's all metadata,
and it can tell you a lot about the book.
But you have to actually read
the book to know what it's all about.
Likewise, you can read about data analytics,
but you have to take this course to earn
the Google Data Analytics certificate,
so keep moving forward to gain that new perspective. 
