
# | FOUNDATIONS OF BUSINESS INTELLIGENCE |

# CONTEXT IS CRUCIAL FOR PURPOSEFUL INSIGHTS

Consider the importance of context from a BI perspective. You’ll explore data limitations, including how to address constant changes and access big-picture insights in a timely manner. You’ll also discover strategies that BI professionals use to anticipate and overcome these limitations. Finally, you’ll develop an understanding of how context influences metrics.

Learning Objectives:

    Explain how to anticipate limitations of data and ensure that they do not detract from stakeholder's intent.
    Describe some of the common limitations of data.
    Verify that data has a purpose and is actionable, as opposed to tracking for the sake of more information.
    Describe the meaning and key takeaways BI analysts and engineers aim to get from a metric or a table.


## Welcome to module 3

Hello. You're about to embark on
another section of the
Google Business Intelligence Certificate.
This is wonderful.
You're really seizing the day.
Seize the day or carpe diem is
a famous Latin phrase by the Roman poet Horace.
He used it to express
the idea that we should enjoy life while we
can maybe even taking
some risks in order to live life to the fullest.
More recently, the acronym YOLO,
for you only live once,
is a common way of expressing the same idea.
Interestingly, the original phrase,
you only live once,
was intended to send a completely different message.
The earliest instances of such quotes in
English literature were actually more of a warning.
Their connotation was that life is precious,
so we should use good judgment,
be careful, and protect ourselves from risk of harm.
This is a great example of
a well-known concept being taken out of context.
But lots of other things can get taken out
of context too, including data.
As a refresher, context is
the condition in which something exists or happens.
If you earned your Google Data Analytics Certificate,
you learned a lot about context and how it helps
turn raw data into meaningful information.
If you'd like to review those lessons,
please go ahead and do so
before moving on to the next video.
It's very important for
BI professionals to contextualize our data.
This gives it an important perspective and
reduces the chances of it being biased or unfair.
During the next few lessons,
we will reexamine context from a BI context.
Then we'll move on to some other data limitations,
including constant change and being
able to see the big picture in a timely manner.
I'll also share some strategies BI professionals
use to anticipate and overcome these limitations.
And we'll learn more about metrics and
how they relate to context.
There's much to come, so let's seize the day and
continue our business intelligence adventure. 



# CONSTANT CHANGE AND OTHER LIMITATIONS

## Reexamine the importance of context

Let's try a little experiment.
Think about what might happen if you showed
this line chart to three different people.
You'd very likely get three different interpretations.
Even if they understood that
line charts are used to show change over time,
one person might assume the x-axis represents a few days,
while another might guess
it's showing a span of many years.
Maybe one person would
assume the five colored lines along
the y-axis represent the sales of different products.
Another may suppose they represent
the purchase patterns of different customer types.
The point is,
a line chart with a title,
a legend for the x-axis and the y-axis,
and each of the data values it contains
is a much more effective data visualization.
When you clearly indicate the meaning of
each item by giving them context,
suddenly this line chart can
be easily understood by others.
Contexts helps eliminate the risk of misinterpretation,
this saves your stakeholders time and ensures they have
accurate information to make
data-driven business decisions.
As you likely know,
in data analytics,
context turns raw data into meaningful information.
When you contextualize,
you put something into perspective,
this involves considering its origin
and other relevant background information,
the motivation behind it,
the larger setting in which it exists
such as a particular time period,
and what it might have an impact on.
Contextualization gives something greater
meaning to help people understand it more completely.
This also supports fairness
and reduces the chance of bias when
your users seek to gain
useful insights from the data you're presenting,
which brings me to context in a BI setting.
In BI, there's another aspect
of context that professionals care about
a lot and that's
contextualizing the tools we create for our users.
One key practice that promotes context is
to put the data being shared in a central location.
Typically, this would be a well-designed dashboard.
Then the second step is ensuring there's
a common method for everyone
to interact with that dashboard.
It's important for stakeholders to be able to easily
understand, access, and use the dashboards you create.
This way, people don't have to go elsewhere or
switch contexts in order to
find the information they need.
That empowers all users to
be much more effective in their work.
For example, let's say a company's finance team
needs a dashboard to analyze
costs across the entire company,
so you design a dashboard that shares
key insights about each department's particular spending.
But then what if it turns out that
the operation department's costs are
revealed to be unusually high?
The finance team would want to be
able to take a deep dive into
that department's spending in order to figure
out the root causes of the cost increase.
It would be important to iterate on your dashboard,
so it includes supporting information
about each department as well.
Another part of building
an effective solution is prioritizing
the cross-functional relationships that
exist within your organization.
It's necessary to consider how
the BI work you're doing aligns
with overall business objectives and
how it will be used by your colleagues.
For instance, if your new BI tool
will monitor five different metrics,
and be used by 10 different stakeholders,
it's important to consider how
each user will access and interpret the data.
Basically, to make an effective dashboard,
it's necessary to first understand how
each particular stakeholder will actually use it.
By taking the time to think this through,
you ensure that you create
one robust dashboard rather
than many less effective ones.
Also, because you've created
a single accessible shared dashboard,
this allows for some great collaboration among users.
For instance, that finance team member may be
dismayed by a seemingly small
five percent year-over-year growth number,
but the salesperson can put that number into
context by pointing out that five percent
is actually a good result and
higher than expected given that
the market segment as a whole was
experiencing a 10 percent decline.
The salesperson can provide
that specific markets context,
whereas the financial analysts would
likely only be aware of broad industry trends.
A single dashboard output can bring
about countless insightful conversations.
Expressing results contextually helps you
confirm that you're using
the right data for the stakeholders.
You'll also know that it's in the correct format,
it can be effectively used and shared,
and the results make sense.
This boosts people's understanding and as a result,
the ultimate business benefits. 


## Why context is critical 

In this lesson, you have been learning about the importance of context in business intelligence. As a refresher, context is the condition in which something exists or happens. For example, in a previous video you considered this data visualization: 

< A line graphic with 5 colours, no info >

This line graph just shows five different lines on a grid, but we don’t have any information about what the lines of the graph represent, how they’re being measured, or what the significance of this visualization is. That’s because this visualization is missing context. Check out the completed version of this visualization:

< A line graphic with 5 colours (Member Type), Y = number, X = year, title "Active Membership Types 2016-2021", legend "Corporate, Individual, Student, Academic, Retired/Lifetime" >

This visualization has all of the information needed to interpret it. It has a clear title, a legend indicating what the lines on the graph mean, a scale along the y axis, and the range of dates being presented along the x axis. Contextualizing data helps make it more meaningful and useful to your stakeholders and prevents any misinterpretations of the data that might impact their decision-making. And this is true for more than just visualization! In this reading, you’ll explore a business case where context was key to a BI project’s success.

The scenario:

The CloudIsCool Support team provides support for users of their cloud products. A customer support ticket is created every time a user reaches out for support. A first response team is in charge of addressing these customer support tickets. However, if there is a particularly complex ticket, a member of the first response team can request help from the second response team. This is categorized as a consult within the ticketing system. The analytics team analyzes the ticket and consults data to help improve customer support processes.

Usually, the consultation request is fulfilled successfully and the first response team is able to resolve the customer’s ticket, using guidance from the second response team. However, sometimes even the second response team isn’t able to fully answer the question or new details about the case require additional insight. In that case, the first response team might ask for another consultation, which is labeled as a reconsult.

This is all important context for a BI professional working with stakeholders who are interested in how well current support processes are working and how they might be improved. If they build reporting tables and dashboards that only track consults and not reconsults, they might miss key insights about how effective the consultation system truly is. For example, a high reconsult rate would mean that more cases aren’t being resolved in the first or second attempts. This could lead to customers waiting longer for their issues to be resolved. The leadership would want to evaluate these processes.

Knowing this context, the BI professional working on this project is able to build out appropriate metrics, reporting tables, and the dashboard that tracks that metric in a way that helps stakeholders make informed decisions about this process. By understanding the business context, BI professionals can create more meaningful reports.

Conclusion:

Context is the who, what, where, when, and why surrounding data that makes it meaningful. Knowing this background information helps us interpret data correctly and visualize useful business intelligence insights for stakeholders. When BI professionals understand the context, choose the right data, and build contextualized visuals to share with stakeholders, they can empower businesses and leadership to make successful decisions.


## Data availability in a world of constant change

In a previous lesson,
you were introduced to some of the solutions in
the business intelligence professional's toolbox.
They include data models,
pipelines such as ETL,
data visualizations, and dashboards.
These are all powerful and exciting solutions,
but only if they have relevant, timely,
consistent, and bias-free data to work with.
This concept is known as data availability.
Data availability describes the degree or extent to which
timely and relevant information is readily
accessible and able to be put to use.
Unfortunately, there are various factors that can affect
data availability and therefore can
compromise the integrity of BI solutions.
In this video, we're going to discuss some of
those challenges as well as ways to address them.
First, some of the most common data availability issues
involve integrity.
If you earned your Google Data Analytics Certificate,
you know that data integrity involves the accuracy,
completeness, consistency,
and trustworthiness of data
throughout its entire life cycle.
Typical issues related to
data integrity include duplicates,
missing information, inconsistent structure,
or not conforming to business rules.
If you'd like to revisit the lesson about data integrity,
feel free to do that now.
Then come back to this video when you're ready.
The second data availability challenge
has to do with visibility.
Data visibility is a degree or
extent to which information can be identified,
monitored, and integrated from
disparate internal and external sources.
For instance, employees working in
a company's operations department might have
no idea what data is stored
in the communications department.
Or someone working in the logistics unit might
have data files that contain lots of great information,
but no one else even knows they exist.
Now on the other hand, when you do
have clear data visibility,
it's possible to achieve accurate and timely insights and
really improve your organization's
responsiveness and agility.
To achieve these goals,
BI professionals will often work with their colleagues
to create a list of data repositories for stakeholders.
You can request a short interview with
the data owners or ask people
to complete a quick online survey
about the data they collect and use.
This is a simple but very useful exercise
to discover the kind of data that is available.
Also keep in mind
data visibility challenges don't
just exist within a company's four walls.
Sometimes BI professionals are
unaware of very useful external data.
As you may know, there are
countless free public datasets,
including government research, climate,
energy and health care studies,
industry surveys, and lots more.
All of these can contribute to a successful BI project.
The third data availability factor to be
aware of is update frequency.
Oftentimes, BI projects
will involve multiple data sources.
It's very common for
disparate sources to refresh at different times,
such as weekly versus monthly.
Let's say a business intelligence professional works
for a pet supply manufacturer
based in Brazil and maybe
they analyze products sales volume by city.
If a retail partner moves from
Rio de Janeiro to Sao Paulo in the middle of July,
all of that month's sales would fall under Rio simply
because the partner's address hasn't
been updated yet in the BI system.
Either the retailer's data
needs to refresh sooner to match
sales data or the manufacturer
should look at all data on a monthly basis.
This is why it's important for
the BI professional to understand how
the update frequency of
different data sources can affect insights.
Even if individual data sources are perfect,
the integration aspect is often pretty messy.
Now we've come to a fourth data
availability challenge, change.
Change is a constant in
pretty much every aspect of
our lives and data is no different.
Data availability may be affected because of a change to
internal procedures such as
a system update or a new record-keeping process.
It may change externally because of
a user interface upgrade or
an adjustment to a particular algorithm.
To address this issue,
BI professionals must have a plan for how they will keep
stakeholders up-to-date on changes
that might affect the project.
They should encourage team members to think about
what tools or methods they're using now,
what could change,
and how it may influence the data being
tracked and how to fill any potential gaps.
Data availability is an important consideration
in the field of BI
and you're likely to spend a fair amount of
time working to address data availability factors.
This video provides an introduction to
some of the most common issues you will encounter.
But there are other things that can
affect the availability of data.
Therefore, it's important to be
realistic about the level of quality you're aiming for.
For many projects, good enough is sufficient.
Just be sure to acknowledge the limitations
and constraints if you take that approach.
As with so many things, it's difficult,
if not impossible, to achieve perfection and that's okay. 


## Data ethics and the importance of data privacy

Recently, you’ve been learning about the importance of context in business intelligence. You discovered that, when you contextualize, you put something into perspective by considering its origin and other relevant background information; the motivation behind it; the larger setting in which it exists, such as a particular time period; and what it might have an impact on. Contextualization also supports fairness and reduces the chance of bias when your users seek to gain useful insights from the data you’re presenting.

Likewise, as a BI professional, you have a responsibility to treat data ethically. Data ethics refers to well-founded standards of right and wrong that dictate how data is collected, shared, and used. Throughout your career you will work with a lot of data. This sometimes includes PII, or personally identifiable information, which can be used by itself or with other data to track down a person's identity. One element of treating that data ethically is ensuring that the privacy and security of that data is maintained throughout its lifetime. In this reading, you will learn more about the importance of data privacy and some strategies for protecting the privacy of data subjects.

Privacy matters:

Data privacy means preserving a data subject’s information and activity any time a data transaction occurs. This is also called information privacy or data protection. Data privacy is concerned with the access, use, and collection of personal data. For the people whose data is being collected, this means they have the right to:

    Protection from unauthorized access to their private data
    Freedom from inappropriate use of their data
    The right to inspect, update, or correct their data
    Ability to give consent to data collection
    Legal right to access the data

In order to maintain these rights, businesses and organizations have to put privacy measures in place to protect individuals’ data. This is also a matter of trust. The public’s ability to trust companies with personal data is important. It’s what makes people want to use a company’s product, share their information, and more. Trust is a really big responsibility that can’t be taken lightly.

Protecting privacy with data anonymization:

Organizations use a lot of different measures to protect the privacy of their data subjects, like incorporating access permissions to ensure that only the people who are supposed to access that information can do so. Another key strategy to maintaining privacy is data anonymization.

Data anonymization is the process of protecting people's private or sensitive data by eliminating PII. Typically, data anonymization involves blanking, hashing, or masking personal information, often by using fixed-length codes to represent data columns, or hiding data with altered values.

Data anonymization is used in just about every industry. As a BI professional, you probably won’t personally be performing anonymization, but it’s useful to understand what kinds of data are often anonymized before you start working with it. This data might include: 

    Telephone numbers
    Names
    License plates and license numbers
    Social security numbers
    IP addresses
    Medical records
    Email addresses
    Photographs
    Account numbers

Imagine a world where we all had access to each other’s addresses, account numbers, and other identifiable information. That would invade a lot of people’s privacy and make the world less safe. Data anonymization is one of the ways we can keep data private and secure!

Key takeaways:

For any professional working with data about actual people, it’s important to consider the safety and privacy of those individuals. That’s why understanding the importance of data privacy and how data that contains PII can be made secure for analysis is so important. We have a responsibility to protect people’s data and the personal information that data might contain.


## Anticipate data limitations

We live in a world where data is constantly being generated. There is so much information out there to learn from. But we also live in a world that is constantly changing, and often the data that we encounter has certain limitations we need to consider as we analyze data and draw insights from it.

Factors of data availability:

Previously, you learned about the importance of data availability, which is the degree or extent to which timely and relevant information is readily accessible and able to be put to use. The factors that influence data availability are:

- Data integrity: The accuracy, completeness, consistency, and trustworthiness of data throughout its life cycle.

- Data visibility: The degree or extent to which information can be identified, monitored, and integrated from disparate internal and external sources.

- Update frequency: How often disparate data sources are being refreshed with new information.

- Change: The process of altering data, either through internal processes or external influence.

Next, you are going to consider the limitations of data that might change the availability and how you can anticipate those limitations as a BI professional.

Missing data:

If you have incomplete or nonexistent data, you might not have enough data to reach a conclusion. Or, you might even be exploring data about a totally different business problem! Understanding what data is available, identifying potential other sources, and filling in the gaps is an important part of the BI process.

Misaligned data:

As a BI professional, you will often use data from different sources. Some of these might be internal sources to the business you’re working with, but they might also include external sources. These sources might define and measure things in completely different ways. In cases like these, establishing how to measure things early on standardizes the data across the board for greater reliability and accuracy. This will make sure comparisons between sources are meaningful and insightful.

Dirty data:

Dirty data refers to data that contains errors. Dirty data can cause errors in your system, inaccurate reports, and poor decision-making. Implementing processes for cleaning data by fixing or removing incorrect, corrupted, incorrectly formatted, duplicate, or incomplete data within a dataset is one way you can prepare for this limitation.

Conclusion:

As a BI professional, you’ll need to understand that sometimes the data you work with will have limitations. This could mean that it doesn’t fit within a certain time range, or it only applies to specific situations, or there are challenges identifying the data you need. Being able to anticipate those issues and consider them when you build tools and systems for your business will allow you to ensure that those limitations don’t stop your stakeholders from getting the data they need to make great decisions and ensure project success!


## Meghna: Beware of bias

My name is Meghna and I'm a business intelligence analyst.
There are several types of biases that an analyst can deal with in regular life,
confirmation bias, selection bias, historical bias and applied bias.
Confirmation bias occurs when an analyst is either exploring or
trying to interpret data to confirm with their prior beliefs.
This can happen at any stage of data analysis, while gathering data for
analysis, while actually doing exploratory analysis or while interpreting the data.
Selection bias can occur when we are dealing with samples which are not
representative of the entire population.
This can happen organically when we're dealing with small datasets or
when the randomization process has not happened.
Historical data bias happens when sociocultural prejudices and
beliefs are mirrored into systematic processes.
For example, if manual systems give poor credit ratings to
a specific group of people and an analyst uses this data to feed
into automated systems this automatic system is now going to either amplify or
actually mirror these prejudices into the results.
Finally, talking about outlier bias.
Averages are a great way to hide anomalies and
outliers while skewing our observation.
Data integrity practices are very important to avoid bias in data.
There are a few tips or things that have worked for
me while I've done my analysis and tried to avoid bias.
First one is record all my prior beliefs and
assumptions before I start my analysis to actually be cognizant of the fact
that I do have these preconceived notions about the data or the process.
Second is to use highly randomized set of data to actually use data which
might be more representative of the analysis than being just convenient.
Third one is to gather more data and
do more research about the opposite side of your hypothesis so
that you are not really ignoring that part or you're not really focusing
on the thing that you believe should be the outcome of your analysis.
And the last one, a very important one is to be cognizant of outliers when
the average analysis says things are looking good in the data,
I think it is time to dig more into the data to understand nuances. 



# MOVE BEYOND DATA LIMITATIONS

## Meaningful metrics

Vanity is an interesting word.
If you look up vanity in the dictionary,
you'll discover that it can mean
both excessive pride and something that is empty,
futile, or without value.
It's intriguing to think that we can be
proud of something that matters very little.
But this does happen sometimes,
especially when it comes to business metrics.
In fact, those of us in business intelligence have
a term for this phenomenon: vanity metrics.
Vanity metrics are data points that are
intended to impress others but are not
indicative of actual performance and
therefore cannot reveal any meaningful business insights.
A well-known vanity metric is
the number of people following a company on social media.
Maybe there are hundreds of thousands of followers
but how many of them are actually making a purchase,
how many of them refer other customers to the site,
and how much revenue do they
actually generate for the business?
Showing off a number just because it's
big, rarely accomplishes much.
And that's why it's critical to
ensure each metric you monitor
is productive, informative, and effective.
For example, some useful business metrics might
include a restaurant's customer loyalty rate,
a manufacturing team's productivity levels,
a fitness center's monthly profits and losses,
or the amount of inventory in a pharmacy's warehouse.
These are numbers that can lead
to useful business insights.
When determining which metrics to include on a dashboard,
BI professionals consider four key things.
First, more information is not necessarily better.
Your stakeholders will appreciate
it if you limit the number of metrics on
your dashboards by including only
those that are critical to project success.
Do this by thinking about user requirements,
what users already know,
and what they need to learn to
help them meet those requirements.
Too many metrics,
especially irrelevant or unnecessary metrics,
can confuse people and devalue your dashboard.
Next, makes sure metrics
are aligned with business objectives.
Consider your organization's specific goals,
then pinpoint which metrics can be
used to support them and measure success.
Confirm that the necessary technologies
and processes are in
place to obtain and analyze
the data you need for each metric.
This is another time to think about
all the factors related to data availability.
Avoid vague or super high level metrics.
Instead, they should be clear and
precise enough to inform a particular action.
The SMART methodology can help you
identify the key metrics
for the particular issue at hand.
As you may know, this tool helps
determine a question's effectiveness.
However, it can also help you refine
metrics based on whether they are specific,
measurable, action-oriented, relevant, and time-bound.
If you earned the Google Data Analytics Certificate,
you learned about the SMART methodology.
Feel free to review that lesson before moving ahead.
As a final point, it's
wise to identify the most important
metric first and prominently
display it at the top of your dashboard.
Then supporting metrics can
drill down into the details below.
For instance, when making a dashboard for a tomato farm,
you might put the number of tomato pallets shipped at
the top because total sales is a key metric.
Then the data that supports pallet shipments, such as
worker productivity and the efficiency of
the harvesting machines would be displayed underneath.
In addition, your users will appreciate
it if you group related metrics together.
For our tomato farmer,
that would mean placing sales data in one section,
production insights in another,
harvest rates in another, and so on.
Keep in mind that the best metrics
highlight two key things,
how the organization is doing,
and what decision-makers should focus on.
In other words, they ensure
your dashboards are never created in vain. 


## How to identify key metrics for a project 

### Choosing your metrics

In a previous video, you learned how business intelligence professionals determine which metrics to include in their dashboards to deliver relevant and actionable data to their stakeholders. In this reading, you’re going to consider how choosing the right metrics can determine the success of a project. You’ll do this by exploring an example of a BI professional identifying key metrics for their project.

There are five key points BI professionals take into account when choosing metrics:

- The number of metrics: More information is not always better. BI professionals limit the number of metrics on dashboards to focus specifically on the ones that are key to a project’s success. Key metrics are relevant and actionable. For instance, if metric X drops, is this good or bad? What action would a user take if it dropped that would be different if it rose instead? Too many metrics that aren’t relevant to the project can be confusing and make your dashboard less effective. The goal isn’t to overload the dashboard to account for every single use case, but 80% of the common use cases.

- Alignment with business objectives: Understanding the business objectives can help you narrow down which metrics will support those goals and measure their success. For example, if the business objective is to increase sales, include revenue in your dashboard. You will most likely not want to include a metric such as customer satisfaction because that is not directly related to the business objective of increasing sales.

- The necessary technologies and processes: It’s important to confirm that the necessary technologies and processes are in place for the metrics you’re choosing. If you can’t obtain and analyze the necessary data, then those metrics aren’t going to be very useful.

- The cadence of data: You have to consider how frequently the data becomes available. If a lot of metrics are delivered at a different cadence and frequency, it becomes difficult to schedule a review.

- Use SMART methodology: If you earned your Google Data Analytics Certificate, you know the SMART methodology is a useful tool for creating effective questions to ask stakeholders. It can also be used to identify and refine key metrics by ensuring that they are specific, measurable, action-oriented, relevant, and time-bound. This can help you avoid vague or super-high-level metrics that aren’t useful to stakeholders, and instead create metrics that are precise and informative.

### An integrated view:

In the BI world, data requires a dynamic and thoughtful approach to detect and respond to events as they happen. An integrated view of the whole business is required. In some cases, metrics can be straightforward. For example, revenue is fairly unambiguous: Revenue goes up, and things are going well! But other metrics are a little more complicated.

In an earlier reading, you discovered the importance of context for the CloudIsCool Support team when measuring their ability to effectively answer customer support questions. As a refresher, a customer support ticket was created every time a customer reached out for support. These tickets were addressed by the first response team at CloudIsCool. Sometimes the first response team needed help answering more complex tickets. They would then reach out to the second response team. This was marked as a consult on the support ticket.

Imagine that the BI professionals working with this team now are trying to decide which metrics are useful in a dashboard designed to increase customer satisfaction ratings for support tickets. Perhaps their stakeholders are interested in monitoring consults to ensure that customers are getting the help they need in a timely manner. So the BI team considers adding consult rate, which is the rate at which customer support agents are asking for help from internal experts, as a metric in their dashboard.

Note that an increasing consult rate could be good or bad. It might mean that customer support agents are being more customer-centric and trying to ensure each customer gets the best answer. But it could also mean that agents are being overwhelmed with complaints and having to offload them onto internal experts in order to keep up. Therefore, consult rate is a metric that doesn’t have a clear direction; nor does it have an obvious influence on the decision-making process on its own. So, it’s not a useful metric for this dashboard. Instead, the BI professionals select metrics that indicate success or failure in a more meaningful way. For instance, they might decide to include a metric that tracks when a support agent experiences missing support documentation. This will help leaders decide whether to create more documentation for agents to reference. Notice how this metric has a clear line of action that we can take based on how high or low it is!

Conclusion:

The ability to choose metrics that inform decision-making and support project success is a key skill for your career as a BI professional. Remember to consider the number of metrics, how they align with your business objectives, the technologies and processes necessary to measure them, and how they adhere to SMART methodology. It’s also important to maintain an integrated view of the entire business and how the information your metrics deliver is used to guide stakeholder action.


## North star metrics

So far, you have been learning about how BI professionals choose the right metrics to measure the success of their projects. BI professionals also use another specific kind of metric to measure the long-term success of the entire business or team; this metric is often referred to as a north star metric. In this reading, you will learn more about north star metrics, how BI professionals choose them, and how they can help a business’s growth over time.

### The guiding star:

A company’s north star metric goes beyond short-term goals– it’s intended to capture the core measurable value of a business’s product or services over its entire lifetime. These metrics are a guiding light that drive a business forward. That’s why it’s called a north star metric– like the north star can be used to navigate the wilderness, these metrics can be used to navigate business decisions and lead a business to growth.

Having this metric as the guiding light for the entire business is useful in three primary ways:

- Cross-team alignment: Different teams have different specialties and focuses that help a business function. They aren’t always working on the same projects or with the same metrics, which can make it difficult to align across the entire business. A north star metric allows all of the teams to have a consistent goal to focus on, even as they work on different things.

- Tracking growth: It can be difficult to understand and track the growth of an entire organization over time without understanding the driving metrics that determine growth. A north star metric provides a long-term measurable data point that stakeholders can focus on when discussing overall performance and growth in a business.

- Focusing values: A north star metric is primarily a guiding principle for a business– it determines what is important to the organization and stakeholders. This means that choosing the right metric to guide a business can help keep the values in check– whether that’s customer satisfaction, number of customers completing the sales cycle, or customer retention.

### Choosing a north star metric

Because north star metrics are so key to a business’s ongoing success, choosing the right metric is a foundational part of a business intelligence strategy. The north star metric has to measure the most essential part or mission of the business. And because every business is different, every business’s north star metric is going to be unique. In order to determine what the most useful north star metric might be, there are a few questions you can ask:

    What is essential to this business’s processes?
    What are the most important KPIs being measured?
    Out of those KPIs, what captures all of the necessary information about this business?
    How can the other metrics be structured around that primary metric?

### Real north star metrics

Because more businesses have begun using north star metrics to guide their business strategies, there are a lot of examples of north star metrics in different industries:

- E-commerce:
    · Weekly number of customers completing the sales cycle
    · Value of daily purchases

- Social media:
    · Number of daily active users
    · Messages sent per day

- Streaming and media services:
    · Number of new sign-ups
    · Total reading time
    · Total watching time
    · Monthly subscription revenue

- Hospitality:
    · Number of nights booked
    · Number of repeat customers

These are just a few examples– there are a lot of potential north star metrics for businesses to choose from across a variety of industries, from tech to finance!

Key takeaways:

As a BI professional, one of your responsibilities will be to empower stakeholders to make business decisions that will promote growth and success over the long term. North star metrics are a great way to measure and guide a business into the future because they allow you to actually measure the success of the entire business, align teams with a single goal, and keep the business’s values at the forefront of their strategy.


## Bridge the gap from current state to ideal state

- Bridge the gap:

Business intelligence professionals continually monitor processes and systems to determine if it’s necessary to make updates for greater efficiency and optimization. These professionals explore ways to bring the current state closer to the ideal state. They do this through a process called gap analysis, which is a method for examining and evaluating the current state of a process in order to identify opportunities for improvement in the future.

Gap analysis involves understanding where you currently are compared to where you want to be so that you can bridge the gap. BI uses gap analysis to do all kinds of things, such as improve data delivery systems or create dashboard reports.

For example, perhaps a sales team uses a dashboard to track sales pipeline progress that has a six-hour data lag. They use this dashboard to gather the most up-to-date information as they prepare for important meetings. The six-hour lag is preventing them from accessing and sharing near-real-time insights in stakeholder meetings. Ideally, the delay should be one hour or less.

- Setting direction with stakeholders:

The first step in bridging the gap is to work with stakeholders to determine the right direction for this BI project. Establishing stakeholder needs and understanding how users are interacting with the data are important for assessing what the ideal state of a system actually is. What needs do stakeholders have that aren’t being met or could be addressed more efficiently? What data is necessary for their decision-making processes? Working closely with stakeholders is necessary to understand what they actually need their BI tools to do.

The BI professionals collect information and learn that, as the company grew, it opened offices across the country. So, the sales teams are now more dispersed. Currently, if a team member from one office updates information about a prospective client, team members from other offices won't get this update until the workday is almost over. So, their goal is to reduce the data delay to enable better cross-team coordination.

- Context and data quality:

In addition to identifying stakeholder needs, it’s also important for the BI professional to understand the context of the data they interact with and present. As you know, context is the condition in which something exists or happens; it turns raw data into meaningful information by providing the data perspective. This involves defining who collected it or funded its collection; the motivation behind that action; where the data came from; when; the method used to collect it; and what the data could have an impact on. BI professionals also need to consider context when creating tools for users to ensure that stakeholders are able to interpret findings correctly and act on them.

It’s also critical that BI professionals ensure the quality and integrity of the data stakeholders are accessing. If the data is incorrect, the reporting tools won’t be accurate, and stakeholders won’t be able to make appropriate decisions — no matter how much context they have been given.

Now, the sales team's BI professional needs to identify data sources and the update frequency for each source. They discover that most of the key data sources update every 15 minutes. There are a few nonessential data sources that rarely get updated, but the team doesn’t actually have to wait until those data sources are updated to use the pipeline. They’re also able to confirm that the data warehouse team will verify these data sources as being clean and containing no duplicates or null fields that might cause issues.

- Building structures and systems:

A large part of a BI professional’s job is building structures and systems. This means designing database storage systems, organizing the data, and working with database governance specialists to maintain those systems. It also involves creating pipeline tools that move and transform data automatically throughout the system to get data where it needs to go to be useful.

These structures and systems can keep data organized, accessible, and useful for stakeholders during their decision-making process. This empowers users to access the data they need when they need it — an ideal system should be organized and structured to do just that. To address the sales team’s needs, the BI analyst in this case designs a new workflow through which data sources can be processed simultaneously, cutting down processing time from 6 hours to less than an hour.

- Sharing findings:

If you are coming to this course from the Google Data Analytics Certificate, you may already be familiar with the share stage of the data analysis process. This is the point at which a data analyst creates data visualizations and reports and presents them to stakeholders. BI professionals also need to share findings, but there are some key differences in how they do so. As you have been learning, creating ways for users to access and explore data when they need it is a key part of an ideal BI system. A BI professional creates automated systems to deliver findings to stakeholders or dashboards that monitor incoming data and provide current updates that users can navigate on their own.

In the sales team dashboard example, the final output is a dashboard that sales teams across the country use to track progress in near-real time. In order to make sure the teams are aware of the updates, the team’s BI analyst shares information about these backend improvements, encouraging all sales teams to check the data at the top of the hour before each meeting.

- Acting on insights:

BI focuses on automating processes and information channels in order to transform relevant data into actionable insights that are easily available to decision-makers. These insights guide business decisions and development. But the BI process doesn’t stop there: BI professionals continue to measure those results, monitor data, and make adjustments to the system in order to account for changes or new requests from stakeholders.

After implementing the backend improvements, the sales team also creates system alerts to automatically notify them when data processes lag behind so they're prepared for a data delay. That way, they could know exactly how well the system is working and if it needs to be updated again in the future.

- Conclusion:

A large part of a BI professional's work revolves around identifying how current systems and processes operate, evaluating potential improvements, and implementing them so that the current system is closer to the ideal system state. Throughout this course, you’ll learn how to do that by collaborating with stakeholders, understanding context, maintaining data quality, sharing findings, and acting on insights.


## Case study: USDM - Selecting key project metrics

In this part of the course, you have been focusing on how business intelligence professionals identify effective metrics for a project. A key part of this process is working with stakeholders to understand their data needs and how those interests can be measured and represented with the data. In this case study, you will have the opportunity to explore an example of how the BI team at USDM worked with stakeholders to develop metrics. 

- Company background:

USDM, headquartered in Santa Barbara, California, collaborates with life science companies across a variety of industries, including biotechnology, pharmaceutical, medical device technology, and clinical. USDM helps its customers, from large-scale companies to small businesses, ensure that their database systems are compliant with industry standards and regulations, and work effectively to meet their needs. USDM’s vision is to bring life sciences and healthcare solutions to the world better and faster—starting with its own company values: customer delight, accountability, integrity, respect, collaboration, and innovation. 
usdm.com homepage

- The challenge:

In this case study, you’re going to explore an example of USDM’s work with one of their clients. The client for this project researches and develops antibody treatments for cancer patients. The client needs analytics that measure the effectiveness and efficiency of their products. However, with the client’s existing database, to get the types of reports they need, they have to access many systems, including facility data, licensing information, and sales and marketing data. All of this data exists in various places, and as a result, developing analysis reports creates issues for the client’s stakeholders. Also, it makes it harder to compare key metrics because so many KPIs needed to be brought together in one place. 

To help better understand how effective their product is and forecast demand, the client asked USDM to help architect a data storage system that could address their specific needs. They needed a system that could bring the data their team needs together, follow industry regulations, and allow them to easily create reports based on key metrics that can be used to measure product effectiveness and market trends. A significant part of this initiative started with the basics: what were the actual key metrics for the client’s team and what data systems did they come from? 

- The approach:

To identify which metrics were most important for the client’s business needs, the USDM team needed to get input from a variety of different people from across the organization. For example, they needed to know what charts the sales and marketing teams who used this data for their reports needed, what their existing processes were, and how to address these needs in the new system. But, they also needed to know what data the product development team used in order to measure efficacy. 

- Illustration of team meeting:

USDM worked closely with different teams to determine what charts they needed for reports, how they were accessing and using the database system currently, and what they were hoping to achieve with the new system. As a result, the team was able to determine a selection of key metrics that represented their client’s business needs. 

These metrics included:

    Sales performance
    Product performance
    Insurance claims
    Physician information
    Facility data

To enact a business intelligence solution there must be both the business interaction with stakeholders and the technical interaction with the architects of other team’s systems. Once these metrics were identified by the client, the USDM team collaborated with other members of the client’s team to begin building a new solution that could capture these measurements. 

But, almost every project comes with unexpected challenges; the database tool the team was using to develop the new system didn’t have all of the features the team needed to capture their must-have metrics. In this case, the USDM team collaborated with leadership to develop a list of requests from the tool vendor, who was able to address their team’s unique needs. 

- The results:

By the end of the project, the USDM BI team architected a data storage system that consolidated all of the data their team needed from across a variety of sources. The system captured the key metrics the client needed to understand their product’s effectiveness, forecast sales demand, and evaluate marketing strategies. The reporting dashboards created with this data storage system included everything the stakeholders needed. By consolidating all of the KPIs in one place, the system could provide faster insights and save the client time and improve efficiency without having to run reports from every individual system. The solution was more automated and efficient—and importantly, designed specifically with their team’s most useful metrics in mind.

- Conclusion:

Collaborating with users and stakeholders to select metrics early on can help determine the long-term direction of a project, the specific needs stakeholders have, and how to design BI tools to best address unique business needs. As a BI professional, a key part of your role will be considering key metrics and how to tailor the tools and systems you create to capture those measurements efficiently for reporting use.


## Wrap-up

And just like that, we've reached the end of another section of this course.
You are discovering so much about business intelligence.
I'm really excited for you, for how far you've come, and for
everything that lies ahead.
I hope you're equally inspired and motivated to keep making great progress.
At this point,
you've gained valuable knowledge about some of the most essential elements of BI.
You've learned about context and how it can help people avoid mistakes,
save time and effort, and confirm that data is accurate and fair.
Context is also important when creating BI tools,
as it enables users to collaborate and
share information that helps make business metrics more clear and comprehensive.
You also explored the concept of data availability and
why it's so important in maintaining the integrity of BI solutions.
And you continue to investigate metrics, as well as the strategies that BI
professionals use when deciding which metrics to include on a dashboard.
Soon, it will be time to apply your BI skills to a scenario based project for
your portfolio.
You will create your own approach to the example situation, and
consider how you would complete each task at your company.
This will be an invaluable tool during your job search.
As always, I encourage you to make the most of the discussion forums.
Sharing ideas and questions is a wonderful way to tap into the world of BI.
But first, you have another graded assessment.
Once again, be sure to check out the reading that lists new glossary terms and
take all the time you need to review videos, readings, and your own notes.
Awesome work, and I can't wait to be with you again soon. 



# GLOSSARY

Data availability: The degree or extent to which timely and relevant information is readily accessible and able to be put to use

Data integrity: The accuracy, completeness, consistency, and trustworthiness of data throughout its life cycle

Data visibility: The degree or extent to which information can be identified, monitored, and integrated from disparate internal and external sources

Vanity metric: Data points that are intended to impress others, but are not indicative of actual performance and, therefore, cannot reveal any meaningful business insights



# REVIEW GOOGLE DATA ANALYTICS CERTIFICATE CONTENT
  
## Context

Context is the condition in which something exists or happens. Context is important in data analytics because it helps you sift through huge amounts of disorganized data and turn it into something meaningful. The fact is, data has little value if it is not paired with context.

Understanding the context behind the data can help us make it more meaningful at every stage of the data analysis process. For example, you might be able to make a few guesses about what you're looking at in the following table, but you couldn't be certain without more context.

    2010   28000
    2005   18000
    2000   23000
    1995   10000

On the other hand, if the first column was labeled to represent the years when a survey was conducted, and the second column showed the number of people who responded to that survey, then the table would start to make a lot more sense. Take this a step further, and you might notice that the survey is conducted every 5 years. This added context helps you understand why there are five-year gaps in the table.

    Years (Collected every 5 years)    Respondents
    2010                                28000
    2005                                18000
    2000                                23000
    1995                                10000

Context can turn raw data into meaningful information. It is very important for data analysts to contextualize their data. This means giving the data perspective by defining it. To do this, you need to identify:

    Who: The person or organization that created, collected, and/or funded the data collection

    What: The things in the world that data could have an impact on

    Where: The origin of the data

    When: The time when the data was created or collected

    Why: The motivation behind the creation or collection

    How: The method used to create or collect it

Understanding and including the context is important during each step of your analysis process, so it is a good idea to get comfortable with it early in your career. For example, when you collect data, you’ll also want to ask questions about the context to make sure that you understand the business and business process. During organization, the context is important for your naming conventions, how you choose to show relationships between variables, and what you choose to keep or leave out. And finally, when you present, it is important to include contextual information so that your stakeholders understand your analysis.


## Data integrity

Welcome back in this video.
We're going to discuss data integrity and
some risk you might run into as a data analyst.
A strong analysis depends on the integrity of the data.
If the data you're using is compromised in any way,
your analysis won't be as strong as it should be.
Data integrity is the accuracy completeness, consistency and
trustworthiness of data throughout its life cycle.
That might sound like a lot of qualities for the data to live up to.
But trust me, it's worth it to check for
them all before proceeding with your analysis.
Otherwise your analysis could be wrong, not because you did something wrong, but
because the data you were working with was wrong to begin with.
When data integrity is low, it can cause anything from the loss of a single
pixel in an image to an incorrect medical decision.
In some cases one missing piece can make all of your data useless.
Data integrity can be compromised in lots of different ways.
There's a chance data can be compromised every time it's replicated,
transferred or manipulated in any way.
Data replication is the process of storing data in multiple locations.
If you're replicating data at different times in different places,
there's a chance your data will be out of sync.
This data lacks integrity because different people might not be using
the same data for their findings, which can cause inconsistencies.
There's also the issue of data transfer, which is the process of copying data
from a storage device to memory or from one computer to another.
If your data transfer is interrupted, you might end up with an incomplete data set,
which might not be useful for your needs.
The data manipulation process involves changing the data to make it more
organized and easier to read.
Data manipulation is meant to make the data analysis process more efficient, but
an error during the process can compromise that efficiency.
Finally, data can also be compromised through human error, viruses,
malware, hacking and system failures, which can all lead to even more headaches.
I'll stop there.
That's enough potentially bad news to digest.
Let's move on to some potentially good news.
And a lot of companies, the data warehouse or
data engineering team takes care of ensuring data integrity coming up.
We'll learn about checking data integrity as a data analyst, but
first assured someone else will usually have your back to after
you found out what kind of data you're working with.
It's important to double check that your data is complete and
valid before analysis.
This will help ensure that your analysis and
eventual conclusions are accurate checking.
Data integrity is a vital step in processing your data to get it ready for
analysis whether you or someone else that your company is doing it.
Coming up, you'll learn even more about data integrity.
See you soon!
