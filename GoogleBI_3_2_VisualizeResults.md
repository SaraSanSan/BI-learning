# | Decisions: DASHBOARDS & REPORTS |

# VISUALIZE RESULTS

You’ll consider the tradeoffs involved with building a BI visualization, and you’ll practice creating charts and visualizations. You’ll also explore effective ways to organize elements within a dashboard. Finally, you’ll identify factors that contribute to processing speed and how to maximize dashboard performance.

Learning Objectives:

    Understand how to gather requirements from stakeholders to build a dashboard.
    Identify obstacles and limitations that dashboards must overcome.
    Learn strategies for answering questions with the appropriate dashboard information.
    Understand a project’s scalability.
    Explain the difference between high granularity and high detail.
    Explore solutions if processing speed could be improved or made more efficient.
    Identify contributing factors to processing speed.
    Set privacy restrictions based on what's appropriate for internal/external availability.
    Translate business needs into dashboard parameters.


## Welcome to module 2

Imagine you're building a dashboard.
You know what questions you need to answer for
your users, and you've built a low-fidelity
mock-up that outlines your plans for what charts you'll
make. Plus, you've identified the appropriate tools to use.
Now, it's time for the next step:
designing the visualizations.
In upcoming lessons, you're going to have
the opportunity to practice
creating charts and dashboards yourself.
You'll start by delving deeper
into the trade-offs you must
consider while building BI visualizations.
Then, you'll apply design best practices
in your BI knowledge to create a chart in Tableau.
Once you complete your chart,
you'll explore effective ways to
organize elements within a dashboard.
You'll use your design skills yet
again, but on a larger scale.
And because a major part of
the BI role includes maintenance in
iteration, you'll learn how to make
changes as the business needs evolve.
This is the order that we'll use to learn
about dashboard design during this section,
but it isn't the only way.
You might prefer to plan
high-level dashboard organization before
getting specific with charts.
That's okay, everyone's design process is different.
Personally, I've learned that you rarely
design the perfect dashboard on the first try.
Sharing your ideas with stakeholders as soon
as possible is a great way to get feedback,
continue learning about the BI goal, and ensure
you don't waste effort focusing on the wrong problems.
The next few lessons will
help prepare you to apply what you're
learning to a realistic business situation,
which you'll do later in this course.
I hope you're as excited as I'm to start
building dashboards. Let's do it. 



# COMMUNICATE CLEARLY WITH VISUALS

## Design trade-offs when building a dashboard

When planning a dashboard,
an essential part of your job as
a BI analyst is determining how to
represent data in the most effective way.
Along the way, you'll often
have to make some tough decisions.
Many of these take the form of trade-offs.
In BI, a trade-off involves balancing various factors,
often by prioritizing one element
while sacrificing another,
in order to arrive at the best possible result.
You witnessed an example of this in
the international sales chart from a previous lesson.
In this view of the chart,
the data is set at a yearly timescale.
Each column represents a year and the height of
the bars represent the total sales for that year.
But dashboards are flexible and can be
changed to present the same data in different ways.
For example, you can modify
the filter setting to a quarterly timescale.
Now, there are several additional bars
displaying more information on a single screen.
Notice that a yearly timescale is more condensed,
so it's more difficult to
interpret what happens throughout the year.
But the data that is available is simple
and easy to follow because it isn't as dense.
Either way, selecting appropriate trade-offs
depends on the ultimate business goals.
For example, if stakeholders want to know
the company's total yearly sales in
a specific region for 2019,
the yearly timescales chart provides the clearest answer.
However, if their question involves identifying which
quarter achieved the highest sales
over the last few years,
then the quarterly timescale chart is best.
Sometimes, a trade-off can be more complex.
Suppose your stakeholder wants to
separate the data by country again,
but they also mentioned that
the dashboard is updating too slowly.
In this scenario, the trade-off in question
is that the user wants the dashboard to do more faster,
something that's challenging, if not impossible.
To arrive at the best possible solution,
you might consider speeding up the dashboard
by pre-aggregating your data with SQL.
As you have learned from the Google Data Analytics cert,
aggregation is the process of collecting or
gathering many separate pieces into a whole.
So, pre-aggregation is a term
BI professionals use to describe
the process of performing calculations on
the data while it's still in the database.
This means reducing the number of
rows or the size of the dataset
before it's used in analysis
or a dashboard. Think of it this way:
if you pre-aggregate the data,
it will be in a state that's
closer to what you ultimately need.
This is because some of
the necessary calculations will
happen before the data is aggregated
in the database and sent to
the data visualization tool. That's the trade-off.
Your pipeline will involve more steps,
but your users will get to
the information they need more quickly.
On the other hand, if you choose to calculate
all of the data once it's in the data viz tool,
this eliminates aggregation from the build process.
The trade-off here is that
your pipeline will involve fewer steps,
but your users may experience slower results.
It's also possible to
pre-aggregate only some of the data,
then calculate the remainder
after it's imported to the data viz platform.
Again, it's all about
considering the stakeholder needs then
balancing the different factors and
choosing which element to prioritize.
Also, note that pre-aggregation comes with another cost:
pre-aggregated data is less flexible.
Imagine that another stakeholder wants to
represent sales data by store size.
If you had already used
pre-aggregation to combine the data by region
— thereby putting all stores together, no matter their size —
you'd have a problem.
How you go about solving this problem
will once again depend on the situation.
If the speed issue can be solved with other methods
or you're completely sure
flexibility won't be necessary,
you can make the trade-off and prioritize
either speed or flexibility.
The best solution isn't always clear.
Sometimes, you'll need to get creative.
That's one of the most exciting parts
of being a BI professional:
finding a creative solution to a difficult problem. 


## Compare scope in different contexts

In a previous video, you were introduced to the idea of scope as it relates to dashboard design. You may have also encountered the word “scope” in terms of project scope. In the business intelligence world, you might find the word scope being used in a variety of contexts. And, as you’ll recall from earlier discussions of context, understanding these contexts is key. In this reading, you’ll get a side-by-side comparison of project scope and dashboard scope and at what stage in a project you will likely encounter these terms. This will help as you encounter scope in different contexts as a BI professional so you know what the expectations are in every situation.

- Project scope VS  Dashboard scope

        Refers to the overall project goals, resources, deliverables, deadlines, collaborators, and stakeholders.
        Refers to the breadth of what a dashboard is tracking, including the amount of time and how many metrics it includes.
        
        Determined by team leadership including project sponsors and managers.
        Determined by BI teams as they consider project and user requirements.
        
        Outlined at the very beginning of a project to determine the overarching aspects of the project.
        Outlined as part of the dashboard creation process based on the specific reporting needs.
        
        Involves working with key sponsors and stakeholders to better understand and align on the entire project and its goals.
        Involves choosing KPIs, how much time should be represented, and how to make important data available and understandable to decision makers through the dashboard.

- Key takeaways

Often, as a BI professional, you will encounter language that means different things in different contexts. By paying close attention, asking questions, and thinking critically, you can ensure that you and your team stay on the same page. In this case, the difference between project scope and dashboard scope is useful to understand as you communicate with stakeholders about their expectations with the dashboard specifically, and not the entire project.


## DeAndrea: Business intelligence in action

My name is DeAndrea, and I'm a Product Operations and Strategy Lead for
Google Wallet.
I support the product management organization in launching
payments products for Google.
I specifically work on the Google Wallet app which
allows users to store their credit cards, loyalty cards, driver's license, and
other items on Android devices.
Business intelligence is used to drive key decisions in an organization.
In my current role within payments,
business intelligence has allowed us to identify what our key markets,
where we should continue to grow and spread Google Wallet.
We look at a lot of different information to try to understand,
is a market ready for a payment solution?
So what's the kind of adoption of devices that will be compatible with
the Google Wallet?
Do stores have kind of offline payments set up where they can accept contact
lists?
And so we use that data in that business intelligence information to figure out if
a market is ready for something like Google Wallet.
Or is there more work to do on the partnership side to ensure that consumers
would have the opportunities at their disposal if they had a Google Wallet to
actually pay contactless in a store.
Anytime you recommend something, people are going to ask to see the data.
They're going to want to know why, what you're saying makes sense.
And there's no way to do that without business intelligence,
without understanding kind of what is feeding the opinion or recommendation, and
why that idea is the best one to go with.
In a previous role, I ran a survey where we asked all of our advertising customers
kind of like, what do you think about your relationship with Google?
Is ad serving your needs or your sales rep serving your needs?
What can we do differently?
What can we do better?
How can we best support and enable your business?
So after we ran the survey, we got a ton of data back.
And so we have lots of different user points that we need to figure out a way to
kind of like aggregate and pull out what's the story.
So using different data tools to draw kind of like what's the summary of
the different qualitative responses that we're getting?
Are they positive or negative, and helping to summarize that at a high level.
I think if you just have raw data, it's kind of not feasible to expect anyone
to kind of read through absolutely everything.
So business intelligence and different data tools and data specialists and
dashboards were used to up level the information to make it easier to filter on
specific teams or specific clients and
also view the numbers and aggregate at a country or regional level.
Business intelligence is a fantastic career path for anyone that is
looking to grow and hone skill sets to be in a leadership position later on.
Stick with it, always have an open mind.
Always continue to learn and grow.
And I'm excited to maybe see you all one day and
work with you all on business intelligence. 


## Case study: Allegis Group - Visualizing key data to understand and advance employee performance

In this course, you learned about the dashboard-building process. You also became familiar with many of the visualization strategies that BI professionals use to answer stakeholder questions. But how does this process play out in the industry? In this case study, you’ll learn how talent solutions firm Allegis Group, headquartered in Hanover, Maryland, used a visualization to monitor the productivity and effectiveness of their new recruiters.

- Company background

Allegis Group is a talent solutions firm comprising several specialized companies that solve business problems for clients across a variety of industries. The firm does this by identifying great candidates for its client companies. Allegis Group recruiters identify talent, and then connect them with career opportunities at client organizations. Each time a candidate is placed, that's considered a sale for Allegis Group. 

To successfully place candidates in client organizations, Allegis Group needs lots of internal BI and data analytics and a good understanding of its clients’ data needs. Quick and effective BI insights are essential to Allegis Group’s daily operations. The following case study explores how a BI dashboard helped Allegis Group leaders solve a sales tracking problem with a clever dashboard. This end-to-end project is an example of the kind of work you might do as a BI professional for organizations like Allegis Group.

- Scenario

The talent recruitment process requires oversight and progress reports. Therefore, Allegis Group conducts its own data analytics and BI research to track the performance of its new recruiters. To challenge assumptions about how long it takes for new hires to meet sales goals, Allegis Group leaders wanted data insights into how each cohort of new recruiters performed within the first year. The goal was to create a dashboard that tracks the sales revenue made by the newly onboarded recruiters. With this tool, Allegis Group would be able to measure the new hires’ ability to bring quality talent to clients. Then, these insights would be communicated to internal company leaders in order to improve processes moving forward.

- The business questions

Through internal brainstorming, Allegis Group leaders confirmed that they needed answers to the following questions:

    How are new recruiters performing over time?
    What are the best months of the year to hire new recruiters?
    Are performance goals for new hires correctly aligned?
    Are new recruiters now finding success more quickly than those hired a year ago?

To answer these questions, Allegis Group’s BI team collected data on how many months recruiters had been with the company. They also collected data on the sales revenue generated by recruiters within their first year. The recruiters were divided into cohorts depending on when they were brought onto Allegis Group’s roster. Then, each cohort could be measured by how much revenue they made based on how long they had been with Allegis Group. This would enable Allegis Group to review and evaluate the success of each cohort over the first year of employment. The dashboard would help decision-makers learn about retention rates, the ideal hiring months, and how to improve overall hiring practices.

- The solution

With these questions in mind and the data gathered, the team began creating the dashboard. They first visualized the main metric, which was the sales (in dollars) per number of individuals in the initial recruiter cohort population. This metric represented the total sales for a month divided by the number of recruiters that were initially hired in that cohort. Then, they defined the data source and created a data view. Finally, they decided on a monthly schedule to refresh and update the data with the cohort’s monthly progress report.

After the team aligned on these elements, they began creating mockups of a visualization. They modeled the visualization after an existing project template, which used a chart with a triangle arrangement of boxes to represent data for each cohort at a given time. This arrangement represented data within a cohort for each row and within a relative month for each column. The BI team knew that this visual design best suited their cohort analysis needs, so it was a simple decision to build their own visualization based on the template.

- Cohort analysis dashboard

The Allegis Group used specific charts to best convey the data. The Financial Times Visual Vocabulary poster includes a guide for choosing chart types based on the relationship you’re trying to visualize; there is also a plain-text version on GitHub.

Then, the team loaded the data into the template and created other charts to answer the business questions. Internally, the team tested the dashboard to ensure its interactive features—such as comparing cohort retention and performance—were working properly. Finally, the team released the dashboard to production. They still had a development version to iterate on, but now they had a fully functional version of the dashboard.

In the BI world, the timeline for completing projects can vary depending on the complexity of the data and the skillset of the team. For this project, the period of time between need-finding and production was about a month.

- The results

The resulting dashboard had several strengths:

    The flexibility to answer each of the team’s questions in one place
    A monthly refresh for continued value
    Quick visual comparison within a cohort (rows) and between different cohorts at the same point in time (columns)
    Interactivity for quick comparisons of cohort retention and performance
    Ease of adding new metrics*

_The team began with one metric (sales per number of individuals in the initial recruiter population) but later added percentage of cohort meeting goal, percentage of cohort remaining, average number of starts, and more._

The main chart of the dashboard visualized which cohorts were high-performing and which needed more support. It was easy to find high-performing cohorts based on color. A darker blue indicated a higher number of hires per number of recruiters in the cohort. The triangle arrangement meant that each cohort could be measured horizontally (within cohort), vertically (by time elapsed since hired to Allegis Group), and by color (average starts per recruiter). This gave the long-term year view that they needed for each cohort’s progress, as well as the comparison among cohorts.

Allegis Group leaders use this dashboard to understand the progression of a typical cohort. They can also find out if some months are better to hire Allegis Group recruiters than other months. For example, if recruiters hired in the middle of the year historically perform better compared to cohorts hired toward the end of the year, management can plan accordingly.

- Lessons learned

As with any complex project, Allegis Group’s BI team learned several lessons about what worked well and what could have been improved in the dashboard creation process. One strength they found was in their presentation: The team went through each visualization of the dashboard with the recruitment team that was going to use it. They were able to communicate initial trends and insights, as well as how company leaders could best use the tool. This collaboration was instrumental in driving adoption of the dashboard.

A difficulty they encountered was that it was challenging to clearly convey the complexity of their metrics to the audience. Their main metric (sales per number of individuals remaining in the cohort for a given month) was misleading without context. While this initially seems like a logical metric to use, it has a survivorship bias that skews the data.

A survivorship bias focuses on only those data points that make it past a selection process and ignores those that didn’t. In this case, the metric ignores the recruiters who didn’t stay with the company. Because it counts only recruiters who stayed with the company, it skews toward higher-performing recruiters. The Allegis Group BI team introduced a second metric (sales per number of individuals in the initial recruiter cohort population) to address this nuance and made clear the distinction between the two metrics.

Another lesson they learned was to embed a how-to video into the dashboard. This could have given the recruitment team a quick run-through of the dashboard’s tools and capabilities, enabling the BI team to focus on effectively communicating insights.

- Conclusion

This example demonstrates how a BI team solved a problem by picking the most appropriate visualization. Choosing a highly specific template enabled the team to visualize the most important data in one chart, rather than in several less effective charts.

This team’s success also illustrates the value of maximizing pre-existing examples in order to create new solutions. Resourcefulness is an important BI skill. Often, the inspiration for a visualization comes from examples from other analyses. Sometimes, a BI professional might have trouble deciding which type of chart to select, so they’ll use a reference sheet, such as The Financial Times Visual Vocabulary poster. It isn’t plagiarism to seek inspiration from other sources, so long as those sources are not proprietary or trademarked.

Conducting research on visualizations is an essential part of being a proactive BI professional. Seeking out community knowledge and continually learning about new BI visualization best practices will help you stay current on evolving trends while building a library of reference materials to guide you throughout your career.


# Start a chart

In this lesson, we're going to start creating a BI
chart. If you'd like, open Tableau desktop or
public to follow along with these steps.
This is completely optional but it will help you get used to the interface.
We will begin by going to Sheet 1 of the workbook and
accessing the chart-building interface.
Then, we'll navigate to the dimensions and measures of your data. Dimensions in
data visualization are qualitative data types that can be used to categorize data.
Some examples of dimensions include names such as customer names,
product names, or locations.
Measures are quantitative data types that can be either discrete or
continuous. In the Google Data Analytics certificate, discrete and
continuous data types are explained in detail.
If you'd like to review those lessons, go ahead and do so.
As a quick refresher, discrete data has a limited number of values and
continuous data can have almost any numeric value.
For instance, the number of students in a class is discrete data.
This is because the class roster is finite and
it's impossible to have a value of, say, 1.5 students.
But measures of continuous data have an infinite set of values that contain
intervals within each value.
Temperature is continuous data because it could potentially be infinite and
it can have any numeric value. In data viz, dimensions and
measures are the important trackable elements to be represented.
One of the many decisions you'll make as a BI
professional is how to encode these
dimensions and measures. In BI, encoding describes the process of translating
dimensions and measures into visual representations of the data. With Tableau,
we can drag a dimension or measure of a data set to one of the encoding
types in the Marks dropdown. Using the previous example,
our ad type dimension might be encoded with color.
This means that lines for each type of ad, such as a 15 second skippable ad, will be
represented by a different color.
If we encode this dimension in a different way,
it will change how the chart is interpreted.
Here's the same dimension encoded with line thickness instead of color. Even
with the legend to explain what each line represents, it isn't easy to understand.
The data encoding brings up another situation where you might have
to make a trade off.
Color is a commonly used type of encoding. For
many people, it's an easy way to distinguish information.
However, people with color blindness may not find certain types of color encoding
very helpful.
BI professionals often refer to guidelines
that explain accessible palates.
Also, in this instance we can consider double encoding the ad type dimension.
For example, we can encode it with color and labels.
The labels also specify the ad types, making our visualization clearer and
more accessible. But this creates yet
another trade off: because we're using labels to represent ad type,
we have more visual elements in the chart.
If you have too many visual elements, the chart might be difficult to understand.
However, in this instance, the added visual elements don't create too much
clutter. This is a smart trade off to make, because accessibility is
such a crucial part of building an effective visualization.
Making a trade off that prioritizes accessibility is a design best practice.
You might have to make other kinds of trade offs while you encode the data in
your visualizations.
When this happens, always refer back to your business question and
stakeholder needs.
With these building blocks,
you can now represent all sorts of BI data in a chart.
Soon we'll expand on chart basics and you'll build your own chart from BI data.
Stay tuned. 


## Design resource guide

If you completed the Google Data Analytics Certificate, then you have already spent a lot of time considering how to create data visualizations. Many of the same principles will apply as you begin to create visualizations and dashboards for business intelligence work. That’s why, in this reading, you’re going to get a checklist of tips and tricks that you can use to guide your design process.

Checklist graphic:

- Use a visualization framework: Frameworks like the McCandless Method and Kaiser Fung’s Junk Charts Trifecta Checkup can help you organize your thoughts about data visualization and give you a useful checklist to reference.

- Choose the right chart: Part of creating effective charts is choosing which type of data visualization works best for your needs.

- Organize your process with design thinking: Design thinking breaks down the design process into five stages: empathize, define, ideate, prototype, and test.

- Consider pre-attentive attributes: Pre-attentive attributes like marks and channels are the elements of a data visualization that people recognize automatically without conscious effort.

- Avoid misleading or deceptive charts: It’s important that the visualizations you create are communicating your data accurately and truthfully.

- Prioritize accessibility: Make your visualizations accessible and useful to everyone in your audience by using labeling, text alternatives, text-based formats, and distinguishing and simplifying elements.

- Apply design principles: There are nine principles of design that you should consider when designing your visualizations: balance, emphasis, movement, pattern, repetition, proportion, rhythm, variety, and unity.

Resources:

- If you’re interested in reviewing any of these concepts, you can check out these resources from the Google Data Analytics Certificate and more: This reading about effective data visualizations covers some basics about creating visualizations.

- This guide to selecting the right visualization has a detailed encyclopedia of chart types and when to use them.

- The Financial Times Visual Vocabulary poster includes a guide for choosing chart types based on the relationship you’re trying to visualize; there is also a plain-text version on GitHub.

- This reading about design thinking breaks down each step of the design process in more detail. 


 ## How to choose the right chart type for your data

In a previous video, you learned about dimensions and measures in data visualization. As a refresher, dimensions are qualitative data types that can be used to categorize data. Measures are quantitative data types that can be either discrete or continuous, and encoding is the act of translating dimensions and measures into visualizations. In this reading, you’re going to learn more about dimensions and measures, different encoding techniques, and a guide to choosing the right chart type for your data.

As a BI professional, you will want to create visualization tools that are self-explanatory so that stakeholders can use them to answer their own questions instead of depending on you—which is why thinking about how you are using these elements is so important.

- Dimensions and measures

Dimensions are inherently qualitative data—this means that they are subjective and explanatory measures of a quality or characteristic. Basically, this is data that records observations about the quality of the data. For example:

    Customer names
    Product names
    Geographic locations 
    Observations
    Interviews
    Reviews

These examples are descriptive; they indicate characteristics of the data that aren’t necessarily represented by numerical data.

Measures, on the other hand, are quantitative. Measures are what you will use to actually count the data and track changes over time. This data can be discrete or continuous—basically, this means they can be represented by numbers with limited or unlimited values. For example:

    Temperature
    Revenue
    Distance
    Weight
    Time

The kind of data you have can actually help you choose what kind of chart would be best to communicate your findings.  Luckily, there is a helpful guide on choosing which type of data visualization works best for your needs. Note that this optional guide includes some primary chart types; there are many other charts and chart variations not shown in the table. If your data matches more than one description, you can create a combo chart that combines more than one visualization type.

- Techniques for encoding

As you have been learning, encoding is the act of translating the information represented by your dimensions and measures into visualizations. The artistic elements you choose communicate things about your data:

    Line: Lines in visualizations can be curved or straight; thick or thin; vertical, horizontal, or diagonal.
    _They add visual form to your data and help build the structure for your visualization._

    Shape: Shapes are a great way to add eye-catching contrast—especially size contrast—to your data story.

    Color: Color can help differentiate different elements of visualization and communicate insights.

    Space: Space is the area between, around, and in objects.
    _There should always be space in data visualizations so that the visualization isn’t too cluttered._

    Movement: Movement is used to create a sense of flow or action in a visualization.

These elements can help you break down the parts of your data visualization and what it is communicating—which will help you develop effective visualizations.

- Key takeaways

BI professionals are often focused on empowering their stakeholders and users with access to the data they need to answer their own questions. They do this by visualizing measures and dimensions in charts that complement their properties. These dimensions, measures, and strategies for encoding will help develop visualizations users understand and use.


## ACTIVITY: Create a chart in Tableau

- Activity Overview

In this activity, you will create visualizations in Tableau based on a BI scenario. If you don’t have a lot of experience with Tableau, this will help you get comfortable in the program. If you do have experience in Tableau, this activity will further your knowledge and teach you BI-specific techniques.

Be sure to complete this activity before moving on. The next course item will provide you with a completed exemplar to compare to your own work. You will not be able to access the exemplar until you have completed this activity. 

- Scenario

Review the following scenario. Then complete the step-by-step instructions.

Imagine that you are asked to build some charts for a business that purchases properties in an area, converts them into rentals, and offers them to people on vacation in Athens, Greece. Your contact gives you some recent data from Airbnb about the rentals in the city. This data includes the price to stay at each listing, the durations of each stay, the locations of these rentals, and more.

Your point of contact asks you to create charts to answer the following questions:

    What is the average price per night in each neighborhood?
    Where in the city are the highest concentrations of currently-available rentals?

In the following steps, you’ll practice working with data in Tableau to create charts that answer these questions.

- Step-By-Step Instructions

Follow the instructions to complete each step of the activity. Then, answer the questions at the end of the activity before going to the next course item to compare your work to a completed exemplar. Pro Tip: Save your work

Be sure to save your work periodically as you complete this activity. This will help you avoid losing work. You can also use the deliverables from this activity for further practice or in your end-of-course project. These projects will help you demonstrate your experience to potential employers.

1. Part 1 - Set up your data

Step 1: Access the data

To access the data for this course item, download the following attachment.

Log into Tableau Public. On your profile page, click Create a Viz.

This will open the Connect to Data window. Load your data into Tableau Public by clicking Upload from Computer, then select the Athens Airbnb Data.csv file you downloaded.

It’s always a good practice to understand your data before you visualize it. Now, take a moment to familiarize yourself with the Athens rental dataset. Note the most relevant columns: Id, Neighborhood, Longitude, Latitude, and Price. Get a sense of what types of data are in each of these columns since you’ll be using them to make charts in the rest of this activity. 

Ask yourself the following questions to help you evaluate the data:

    Which columns are string data and which are text?
    Is any data missing?
    Do any names or IDs occur particularly often?
    Are there any unusually high or low values in the Price column?

Part 2 - Build your first chart

To create a new chart, click the tab for Sheet 1. This will open the chart-building interface where you can begin placing dimensions and measures into their respective places.

Because the client’s priority is finding out the average price of each rental per night in each neighborhood, you’ll build that visualization first. Click and drag the Neighborhood dimension next to the Columns field at the top of the screen.

Then, drag the Price measure to the Rows field. This will update the visualization to represent the sum of the price in each neighborhood. This could be a good metric to estimate which neighborhoods are the highest-grossing, but it won’t tell you if this is because there are lots of rentals there or just a few high-priced ones. 

Instead, change SUM(Price) to AVG(Price). Right-click it, hover over Measure in the dropdown, and select Average.

When you do this, you’ll get a bar chart that represents the average price per neighborhood. One of the bars in this chart is significantly taller than the others, which indicates that it’s a significant outlier.
This bar chart represents each neighborhood’s average rental price. The outlier makes the chart more difficult to read.

You might notice a significant outlier in this chart. One of the entries far outscales the other entries, making it hard to focus on trends in the chart. Outliers are important to identify and keep in mind, but in situations like this it helps to temporarily remove them from the view. This won’t change the data itself, so you won’t introduce bias to your analysis, but it will make your chart more proportional and help you notice trends.

To do this, click on the bar that corresponds to the outlier value. Select Exclude to update the chart and view it without the outlier.

You can also do this by clicking on Measure and choosing Edit filter.  From this window, select the value you’d like to exclude and click OK.

Either of these methods will create a filter for Neighborhood. To include the outlier in the visualization again, undo the steps you took or right-click and delete the filter itself. Even if you aren’t representing outliers in your charts, you should make note of them when presenting your visualization to your stakeholders.

< Bar chart comparing the Average Price Per Neighborhood >

Step 3: Order the data

Removing the outlier helped rental price trends stand out, but there is one more step to take before presenting the data to your stakeholders. Ordering the bars in the chart from highest to lowest visualizes the data in a way that’s easier to interpret at a glance. 

To do so, select the table header, Neighborhood, then right-click and select Sort descending from the dropdown menu. 

< A dropdown menu showing two sorting options: ascending and descending. >

After it’s sorted, the bar chart data will be arranged to represent the neighborhoods with the highest average rental price to the neighborhoods with the smallest average rental price. 
This bar chart has been sorted to show most expensive to least expensive neighborhood rentals.

3. Part 2 - Build a map chart

Now create a second chart. This time, you’ll create a map that visualizes the concentrations of where rentals are located within Athens. This will help your stakeholder identify which neighborhoods are most popular so they know where to buy properties to turn into rentals.

To begin, create a new worksheet by clicking the New Worksheet next to Sheet 1. You can also do this by clicking Worksheet in the menu and selecting New Worksheet. 

Note: It’s a good idea to rename each worksheet as you create it. If you haven’t already, right-click Sheet 1 to name it “Average Price per Neighborhood.” Then, rename Sheet 2 to “Rental Map of Athens.” This will help you find each chart when you need to arrange them into a dashboard in an upcoming activity.

To make your map, start by dragging Longitude into the Columns field and Latitude into the Rows field. At first, Tableau will represent these as averages. Since you want each data point to be discrete, right-click Longitude and select Dimension in the dropdown instead of Measure. Do the same for Latitude. Now, your map will show a dot for each rental location.

This map displays blue dots to represent locations based on Longitude and Latitude.

At this point, because all the dots on the map are the same size, it’s hard to tell where each one begins and ends.  You can change the size of each dot to reflect the number of times each property ID appears in an entry. This will indicate which properties have been booked the most.

To do this, drag the Id dimension to the Size square under the Marks dropdown. Then right-click Id, hover over Measure, and select Count.
This map represents rental locations. The size of the dots represents the frequency of each ID in the data.

Now that your data points are properly in your map, there are some visual elements you can change to make your map easier to read.

First, click on Map in the toolbar. In the dropdown, select Background Layers and the layers window will appear on the screen.

Under style, select Streets instead of Light. Including highways, roads, neighborhoods, and other features of the city of Athens will make your visualization appear more like a traditional map. It will also place your data points within the context of their surroundings. 
This map represents rental locations. It has highways, roads, neighborhoods, and more.

This way, your map is more useful than a collection of dots on your screen. You can also zoom in with the + and - icons to focus on specific parts of the map.
This map represents rental locations. The map is zoomed in to display more detail.

If you haven’t already, take a moment to save your work in Tableau Public. Click File in the toolbar and then select Publish. Make sure to publish your work before clicking the X icon in the corner. The publish option functions as a save, and you can always change the privacy settings after your work is saved and published. In an upcoming activity, you’ll need to start a dashboard using these charts, so it’s important to keep them in a place that’s easy to find. 

If you do not want to publish your charts publicly, publish your work, and then click the X icon in the upper right corner. This will take you to the shareable view page on Tableau Public. To stop sharing this project on your public profile, click the settings wheel. You can toggle the Show Viz on Profile option as well as the Allow Access option. 
The settings menu allows different options for sharing visualizations. The menu is currently set to show the visualization on

If you’d like to download your work, click the download icon. This will give you several file formats to choose from. To save your work in a format you can use directly in Tableau Public later on, select the Tableau Workbook file format.

- What to Include in Your Response

Be sure to address the following elements in your completed charts: 

    A chart that visualizes Average Price per Neighborhood with Neighborhood in the Columns field and Price in the Rows field.
    A map that visualizes Concentration of Rentals with Longitude in the Columns field, Latitude in the Rows field, and CNT(Id) as the size modifier.


## Activity Exemplar: Create a chart in Tableau

As a business intelligence professional, you will often design and create visualizations to showcase data findings to stakeholders. In the previous activity, you used Tableau to create visualizations to help answer two questions for a rental hosting business in Athens, Greece:

    What is the average price per night in each neighborhood?
    Where in the city are the highest concentrations of currently available rentals?

To design visualizations that could answer these questions, you accessed and explored the data to determine what metrics had been captured. Then you took the stakeholder’s questions into consideration as you created a bar chart to determine the average price of each rental per night in each neighborhood. You removed an outlier from the visualization to make sure your findings weren’t skewed in the report. And finally, you built a second visualization to demonstrate the concentration of rental properties on a map.

Your charts don’t have to match the exemplar exactly; with these activities, the goal is for your work to achieve the same results, even if you found another way to solve the problem. Basically, this is an opportunity for you to check for understanding, ensure that you’ve met the activities expectations, and explore one possible solution.
This bar chart has been sorted to show most expensive to least expensive neighborhood rentals.

< Map of rentals in Athens, Greece. >

Now that you’ve accessed the exemplars, take a moment to compare them to the charts you created. In the exemplar, you will find that this BI professional followed the steps from the activity to create multiple visualizations that allow stakeholders to clearly answer the two questions established in the activity:

    What is the average price per night in each neighborhood?
    Where in the city are the highest concentrations of currently available rentals?

Your work should achieve the same basic use-case, even if it appears slightly different from this exemplar version.

- Key takeaways

Being able to recognize what visualizations are useful for presenting data and creating charts based on the questions your stakeholders ask is a large part of a BI professional’s work. Coming up, you are going to have an opportunity to take your reporting one step further and use these charts to create an interactive dashboard that your stakeholders can access themselves.



# CONSIDERATIONS WHEN LAYING OUT A DASHBOARD

## Organize dashboard elements

Recently, you've been learning
how to design charts in Tableau.
Now, it's time for the next step:
organizing a dashboard.
In this video, you'll
shift your focus from the details of
a single chart to design
approaches for an entire dashboard.
You'll learn many of the same design principles,
but on a larger scale.
In Tableau, organizing your charts
(sometimes called worksheets) into
a dashboard is fairly simple.
Let's check it out. To create a new dash,
we'll drag the relevant charts to
the center dashboard design interface.
Once the charts are placed onto the dashboard,
we'll rearrange them in a configuration
that best suits the stakeholder needs.
Suppose that stakeholders at a university want to expand
the course offerings to cater to
the demand of prospective students.
So the administration ask for
a dashboard tracking the most popular courses each term.
We want to place the chart that tracks popular courses at
the top because it's the most important chart
and the most relevant.
But we might also want to include a chart
that displays more general admissions data,
as well as one that shows the popularity of
courses from other nearby universities.
This will enable us to monitor the education landscape.
Where might we put these charts?
Some of these placement decisions may have already
been made during the mockup planning stage.
Make sure to reference the low fidelity drafts
when building visualizations.
Also, consider previous discussions with
stakeholders about their needs and
relevant metrics and KPIs.
Ok. Now there are many other elements
that can be included in a dashboard,
such as titles, labels,
a legend, and a navigation bar to help direct users.
The Google Data Analytics certificate
has lots of lessons about this,
so feel free to do a quick review.
We can also include links to webpages or
internal documents that a stakeholder
may want to reference.
Once we have an idea of the dashboard elements,
it's time to apply design best practices.
You've already reviewed several of
them earlier in this section.
While we should make sure to use each of
the best design practices at our disposal,
a few of them will be particularly helpful for building
BI dashboards that don't overwhelm the audience.
One of these practices is prioritization and hierarchy.
If we have a visualization tracking data
that is highly relevant to the stakeholders' question,
we can emphasize it visually.
Do this by increasing
its size compared to other visualizations.
A larger chart naturally draws
more attention than a smaller one.
Also, use color and
negative space to highlight important elements.
Colors with more contrast
are more likely to get noticed,
and negative space can emphasize
an element within empty surroundings.
Grouping objects that share a topic or tell
a story helps ensure that
our dashboard has a logical flow.
For example, we might keep financial data in
a single place rather than disbursed throughout the dash.
Then we can put time-related data in another area.
Another helpful design tip is to hide objects.
It might sound counter-intuitive to
create a visualization and then hide it.
But we can organize visualizations
on multiple pages or place them
within drop-down menus that hide
parts of the dashboard from the main screen.
By hiding some elements,
we can spotlight others,
avoid clutter without deleting
content, and even increase processing speed.
You'll learn more about that soon.
One final point, don't group objects based on chart type.
Putting all of the bar charts together simply
because they are bar charts isn't a useful practice.
Instead, organize by topic or metric.
Soon, you'll get an opportunity to apply
these design practices and build
your own dashboards. Can't wait. 


## ACTIVITY: Lay out dashboard elements in Tableau

- Activity Overview

In this activity, you will use Tableau to build a dashboard. To do this, you will use the charts you made in a previous activity.

You might have built a dashboard before, but now you will explore more design elements you can include to enrich your dashboard.

Be sure to complete this activity before moving on. The next course item will provide you with a completed exemplar to compare to your own work. You will not be able to access the exemplar until you have completed this activity. 

- Scenario

Review the following scenario. Then complete the step-by-step instructions.

In a previous activity, you built some charts for a business that buys homes to convert them into rentals in Athens, Greece. You made a chart using data from Airbnb to represent the average price of listings in the area. Then you made a map to represent the concentration of listings in the city. These charts answered the following questions from your stakeholders:

    What is the average price per night in each neighborhood?
    Where in the city are the highest concentrations of currently available rentals?

Now, you’ll arrange the charts you made into an interactive dashboard that answers your stakeholders' questions. 

- Step-By-Step Instructions

Follow the instructions to complete each step of the activity. Then, answer the questions at the end of the activity before going to the next course item to compare your work to a completed exemplar. Pro Tip: Save your work

Be sure to save your work periodically as you complete this activity. This will help you avoid losing work. You can also use the deliverables from this activity for further practice or in your professional projects. These projects will help you demonstrate your experience to potential employers.

1. Part 1 - Open your charts in Tableau

Go to Tableau Public and open the charts you published in the activity Create a chart in Tableau. 

You used the Athens dataset to make your charts. To access this dataset again, download it from the following attachment.

2. Part 2 - Organize your dashboard

Go to Sheet 1. You might have renamed it “Average Price per Neighborhood.” This will be the first chart you bring into your dashboard. 

To make your dashboard, click the New Dashboard icon. You can also click Dashboard in the toolbar, then select New Dashboard. This will create a new dashboard and display your charts (known as Sheets in Tableau Public) in a menu.

From here, drag the Average Price per Neighborhood chart onto the dashboard interface. It will take up the majority of the interface.

< A Tableau dashboard with a bar chart included. The bar chart compares the average price per neighborhood. >

Now, you’ll do the same for the map you created. Drag Rental Map of Athens from the menu to one side of the screen. You’ll find that the highlighted box previews where you’re going to place the chart.

< A tableau dashboard with a bar chart displayed. The right half of the bar chart is shaded. >

Once you drag the map into the dashboard, it will populate next to the bar chart and include a legend to describe what each dot size on the map means. 

Note: If you ever place a chart in the incorrect location, you can always move it again by dragging it to the place you want it.

< A rental map of Athens sits to the right of the bar chart. >

3. Part 3 - Use your dashboard

In this activity, you are making a simple dashboard with only two charts. Future dashboards you’ll make later in this course and in your professional roles might be much more complex. For now, you’ll use this simple example to practice Tableau skills and demonstrate how BI visualization software like this can expand your data capabilities. 

One of the many things Tableau can do is make your charts interact with each other. For example, you can highlight a certain portion of your map and update the chart next to it to only reflect average prices for that location.

To do this, click and drag on the interface of the map you created. You can select any portion of the map, but the smaller the area you select, the fewer bars will display in the bar chart. 
A small selection of dots are highlighted on the map. They represent a subsection of the map data.

Once you have highlighted a portion of the map, click the map’s filter icon. This will automatically update the bar chart to display only the prices from the location you’ve highlighted.
The filtered bar chart now has only three bars for the data points that correspond to the highlighted map section.

Note: This option only shows if the chart is selected. If it is not displaying correctly, click on the map’s title. 

4. Part 4 - [Optional] Create more visualizations

Now that you’ve started your dashboard, you’ve completed what is required for this activity. However, you are encouraged to discover more features of Tableau on your own. You might create more charts and arrange them in your dashboard. You might add other objects to your dash or create another layout for its mobile version. While you will learn many helpful tips in this course, it’s also important to explore the software and seek out tutorials on your own. Challenge yourself to add an additional component to your dashboard that you weren’t instructed to add.

- What to Include in Your Response

Be sure to address the following criteria in your completed dashboard: 

    Dashboard contains the bar chart made in the previous activity
    Dashboard contains the map made in the previous activity
    A portion of the listings map is highlighted
    The bar chart displays only a subsection of the data (has fewer than the total amount of bars)

- Key takeaways

As a BI professional, a large part of your job will be designing dashboards that empower users with meaningful data that allows them to answer their own questions and make informed decisions. These insights are key to business intelligence, so designing dashboards that incorporate interactive visualizations that guide business decisions will be a key skill you’ll use a lot in your future career!


## Processing speeds and privacy settings

As you know, delivering a dashboard to
your clients is not the end of your role in a project.
BI involves a lot of iteration,
often based on stakeholder feedback,
in order to get closer and closer to the ideal end-state.
Users might share comments about
your aesthetic choices or your design approach,
or, as we've explored in many examples,
clients may have feedback about access and privacy,
as well as processing speed.
Speed is critical in BI.
Let's begin by identifying some common causes of
slow processing speed and learn how to fix them.
You've probably figured out that
processing speed describes how
quickly a program can update and
load a specific amount of data.
If the load is too high,
then processing speeds will be slow,
and the tool might even crash.
This can make it difficult or
frustrating to work with the dashboard.
Of course, the greatest contributors to high loads and
slow processing speeds are the volume of
data and the number of measures and dimensions included.
Naturally, the more data,
the greater the volume of information being
processed and visualized at a given moment.
Also, the number of tabs in
a dash can affect processing speed.
If there are several tabs,
you can better organize your visualizations.
However, having too many tabs may slow things down —
yet another BI trade-off.
Begin considering how to reduce load and
increased processing speed at the start of your planning.
As a rule, you should begin broadly,
then narrow your scope.
In other words, identify the priority KPIs,
then consider and refine supporting information.
Along the way, you might
find that a metric you were originally
asked to track is no longer
relevant to your stakeholders' business question.
In this case, you can remove it from your dashboard,
which will help things move more quickly.
In addition, you can optimize
processing speeds by changing
calculations in your database.
This enhances dashboard efficiency
because back-end servers are more
powerful than front-end servers
and can process more data faster.
However, if a calculation is
dependent on the filters applied in its dashboard,
then it can only be completed
within the dashboard itself.
This is an uncommon situation
for entry-level BI professionals,
but one that's important to be aware of.
Configuring the amount of data
that is preloaded in the dashboard,
can also be a good solution.
Preload less data and
there will be less strain on the dash.
But keep in mind that preloading may mean
that the insights aren't as current as they could be.
Other strategies for speeding up your dash include
filtering data early on and pre-aggregation.
You learned about that earlier in this section.
Ok, now let's turn our attention to another important part of
the dashboard iteration process: privacy.
As you know, a dashboard may be used
by many stakeholders within a company.
Often, certain data is available to some people,
but others don't have permission to access it.
As a BI professional,
configuring privacy settings is
a crucial part of building and maintaining dashboards.
There are several types of privacy permissions,
but we're going to focus on three main levels:
public availability,
object level permission, and row-level permission.
If your dashboard is publicly available,
it's accessible to anyone.
Use this unrestricted setting to
share dashboard with the general public.
The next is object- level permission.
This privacy setting controls
the availability of a single item,
such as a table, dataset, or single visualization.
You'll probably employ object level permission the most,
due to their simplicity.
If you give a user access to an object,
revoking that access is as
easy as removing their permission.
The third permission type is row-level.
Row-level permission is a privacy setting that controls
the availability of specific rows of a table or dataset.
This type of privacy setting is a bit more complex,
because it must be set up in
the database rather than the visualization tool.
Configuring complex permissions, where data from
several sources is selectively
available to different groups,
is something that even some
experienced professionals find difficult.
You likely won't need to understand
every detail about permissions when starting out in BI.
You may even be on a team with
a data engineer who will work
with you to configure permissions.
For now, you've learned some important fundamentals
about iterating dashboards based on stakeholder feedback.
Next, you'll get the opportunity to continue
applying this knowledge to your own dashboards.
I hope you're as excited as I am. 


## Reduce processing load and maintain dashboard effectiveness

Previously, you learned about the importance of optimizing processing speed for dashboards. Processing speed describes how quickly a program can update and load a specified amount of data. Basically, it’s how fast your dashboard can deliver answers to users. Processing speed is usually determined by the volume of data, the number of measures, and the number of dimensions. This is another example of a trade-off: you have to balance various factors, often prioritizing one element while sacrificing another, in order to arrive at the best possible result. In this case, there is a trade-off between processing speed and workload. This reading will offer solutions that enable you to reduce processing load while maintaining the effectiveness of your dashboard.

- Reduce processing load

One of the primary ways you can work to optimize your processing speed is by reducing the processing load. You can do this by:

1. Pre-aggregating: This is the process of performing calculations on data while it is still in the database. Pre-aggregating data will transform data into a state that’s closer to what you ultimately need because some necessary calculations will happen before the data is sent to the data visualization tool. The trade-off is that your pipeline will involve more steps and your dataset uploaded into the visualization tool will be less flexible , but your users will get the information they need more quickly.

2. Using JOINs: JOINS are used to combine rows from two or more tables based on a related column. This basically merges tables together before they’re ever used in the dashboard. This can save a lot of processing load in the actual dashboard. However, if you are trying to join a full table, it can be more of a burden to the system. This is caused by the dimensionality of the tables. For example, joining a one million row table with a 100 million row table will most likely generate a lot of overhead every time the dash is updated. So it’s important to think carefully about how you use JOINs to reduce processing load!

3. Filtering: Filtering is the process of showing only the data that meets a specified criteria while hiding the rest. Filtering the data early in your dashboard’s processing means that it doesn’t have to sort through data that isn’t actually going to be used. The tradeoff of this is that this means less data is available for your users to view on their own.

4. Linking to external locations: In cases where you have data in your dashboard that you can provide context for outside of the dashboard and which can help cut down on the processing load, you can link out to that location for users to explore on their own.

5. Avoiding user-defined functions: Users making requests of your dashboard can add a lot of load to the processing work it’s doing. Consider the kinds of questions that users might have when designing the dashboard so that you can address them without the users themselves having to input functions repeatedly.

6. Deciding between data views and tables: Tables contain actual data. Data views are the result of a stored data query that preserves business logic and can be queried like a database. Data views often require much less processing load because they don’t contain actual data, just a view of the data. This makes them less flexible, so you’ll want to consider how interactive you need the data in your dashboard to be.

- Key takeaways

When you are considering dashboard design, you’ll have to consider processing speed and load and decide how to best balance them to deliver the answers your stakeholders need as quickly as possible. This can be challenging, but you can apply the strategies described in this reading to reduce processing load and improve performance.


## Case study: FeatureBase, Part 3: Exploring the trends with visualizations

In previous courses, you learned about FeatureBase, an OLAP database company that solved a problem with their sales cycle. FeatureBase found that customers were leaving in the early stages of the sales cycle and not converting to paying customers. In this case study, you’ll learn about what came after the sales team made their findings: visual insights that helped FeatureBase solve their business problem.

- Company background

As a refresher, FeatureBase is an OLAP database company that enables businesses to gain insights from real-time analytics and AI. Their core technology, FeatureBase, is the first OLAP database built entirely on bitmaps that power real-time analytics and machine learning applications by simultaneously executing low latency, high throughput, and highly concurrent workloads. FeatureBase is sold to their clients, who become part of the sales cycle. This cycle includes the first point of contact with the potential customer to the moment they sign the purchasing contract and begin using FeatureBase.

- The challenge(s)

As you learned in the previous case study, the FeatureBase sales team realized that they didn’t have the data they needed to find when customers were falling off. To fix this, they recreated their original sales funnel with new attributes that helped track customers at every stage of the sales cycle.

Their next challenge was deciding the best way to visualize the problem for the sales team.

- The approach

FeatureBase selected an informal series of simple charts rather than a dashboard to help make fast decisions. This allowed the sales team to find the most difficult stage of the sales cycle in a matter of minutes, rather than requiring at least a week of dashboard creation. While many complex business questions are best answered with a carefully-crafted dashboard, this problem required a simple visual solution.

FeatureBase’s sales team used DataStudio to create a simple line graph that tracked the conversion rate from each stage to the next. The first data point on the left would represent 100% of the potential customers that began the sales cycle. At each following stage, represented on the X axis, the data point would represent how many potential customers converted to the next step of the sales cycle.

< A line graph representing conversion rate for each sales cycle stage. There is a decrease at the technical validation stage. >

With this, they confirmed that a significant amount of customers dropped off at the technical validation stage. The line graph they made had a significant drop between the technical validation stage and the contract stage – meaning that a large portion of users backed out of the sales process because they didn’t complete the technical validation process.

This stage is the point at which FeatureBase would be implemented in the customer’s data environment to determine if it was actually functional for them. At this stage, the sales team could showcase FeatureBase’s utility and provide proof that it would be a workable solution for their customer.

With this insight, they could infer that either the technical validation stage had a fundamental problem, or the clients were having trouble understanding the highly-technical aspects of FeatureBase.

- The results

Once the sales team knew that technical validation was the likely stopping point for their customers, they wondered if only certain types of potential customers were experiencing difficulty. They created a bar chart that represented different channels, or types of clients.

< A bar chart representing the percent of clients in each channel that result in a sale. The software bar is the tallest. >

With this bar chart, FeatureBase’s team found that companies or points of contact who had non-technical backgrounds were the ones that were less likely to proceed to the contract stage. Then the sales team made a pie chart to confirm their suspicions. This pie chart offered evidence that an evaluator with a non-technical background was less likely to sign contracts.

< A pie chart of the converted sales by channel type. Technical channels are a larger portion than the non-technical portion. >

- Conclusion

By visualizing the data, FeatureBase’s sales team and leadership found that their technical validation stage might be too confusing for non-technical clients and that selling to them is less likely to be successful. Using this insight, the team pivoted to focus on turning users into “champions” that would then advocate for the product and “sell” it to their business unit leaders. These champions could help their teams understand how to use FeatureBase and answer questions that might otherwise discourage clients. What started as a question to be answered eventually led to a business strategy change where the BI professional played a critical role in helping FeatureBase make a data-driven decision. The sales team was able to answer this question with just a few charts. In this situation, a huge dashboard would have taken too long to create. The team’s priority was finding the source of the drop off as quickly as possible, so a simple solution was most effective. 

In your role as a BI professional, you may find that the traditional solution isn’t the best one for every situation. It’s your job to determine the best way forward by applying your BI knowledge and creative thinking to each of your projects. 


## Privacy settings in business intelligence tools

As a business intelligence professional, you won’t just create dashboards and visualizations. You will also share these tools with stakeholders so that they can access the data to get up-to-date information and make informed decisions. You empower stakeholders with the ability to answer their own questions—but you also want to ensure that only the people who are supposed to access that information can do so. This has to do with data privacy and security. In this reading, you will learn about some of the privacy restrictions that are already included with Tableau as well as other common BI tools.

- Privacy settings in Tableau

Incorporating privacy settings in your dashboard helps ensure that the data remains secure, even when people from across your organization need to access it for different purposes. Throughout this program, you will be using Tableau to practice key concepts and get familiar with sharing BI insights. Luckily, Tableau already has a variety of privacy and security settings built in that you can take advantage of.

- Setting permissions

Tableau gives you the power to set permissions to control how users are interacting with your dashboards and data sources; you can even use permissions to determine which users can access which parts of a workbook. Tableau organizes permissions into projects and groups. Basically, this means you can determine permissions depending on project needs, or by groups of users instead of person-by-person.

You can also use permission settings to choose what metrics users can interact with, show or hide different sheet tabs, or even add explanations of the data that can be seen by different users depending on their specific needs.

To learn more about permissions and how to set them yourself in Tableau, you can check out the Tableau Online Help article about permissions.

- Managing user visibility

In addition to allowing you to determine what permissions users have as they interact with your Tableau dashboards, you can also manage how users are able to interact with each other. Usually, all users can view other users’ aliases, project ownership, and comments by other users by default. But in cases where you have created a tool that’s being used by multiple clients, teams, or users who don’t need to interact, you can actually determine how much visibility users have of each other.

To learn more about user visibility settings and how to set them yourself in Tableau, you can check out the Tableau Online Help article about managing user visibility.

- Row-level restrictions and filtering

Finally, Tableau allows you  to filter the actual rows of data so users can access the data relevant to their role without having to create an entirely separate view for them. This is especially useful when working with live data sources or extracts that use multiple tables.

To learn more about user visibility settings and how to set them yourself  in Tableau, you can check out the Tableau Online Help article about user filters and row-level restrictions.

- Privacy settings in other tools

Other tools that you might encounter as a professional also use privacy settings that allow you to determine what data different users can access and view. Here are some resources you can use to learn more about those tools:

1. Data Studio: Sharing, access permissions, and data credentials

2. Looker: Access control and permission management

3. MicroStrategy: Restricting access to data: security filters

4. PowerBI: Power BI Desktop privacy levels



# Review: VISUALIZE RESULTS

## Wrap-up

Congrats on completing this section.
You're really making excellent progress.
You've learned more about the tradeoffs involved in building a dashboard and
how they affect data visualization. By understanding these tradeoffs and
making the right decisions about them,
you can answer your stakeholders questions more efficiently.
You also explored how to design a BI
chart. This lesson expanded on your prior data
viz experience by focusing on flexibility and interactivity.
Once again, you learned about the kinds of trade offs you might make while encoding
your data's dimensions and measures.
Next, you organized charts and other BI elements into a dashboard.
You considered how to apply these design best practices to make clear and
concise dashboards that effectively answer business questions. And
you delved into the impact of processing speed and
how it contributes to usability and responsiveness.
You also investigated the different privacy permissions which affect
how you work with your data and share it with stakeholders. Coming up, you'll
get more practice creating dashboards and apply your design skills and BI
experience to a realistic business scenario.
But before that, you have another challenge.
This was a hefty chapter with a lot of material to cover.
But not to worry — if you need more time to review you can always return
to the videos, readings, activities, and practice quizzes. And of course, be
sure to check out new entries from the latest glossary. When you're ready,
proceed to the graded assessment.
Good luck. 


## GLOSSARY

Dimension (visualization): A qualitative data type that can be used to categorize data

Encoding: The process of translating dimensions and measures into visual representations of the data

Measure: A quantitative data type that can be either discrete or continuous

Object-level permission: A privacy setting that controls the availability of a single item in a dashboard

Pre-aggregation: The process of performing calculations on data while it is still in the database

Processing speed: How quickly a program can update and load a specified amount of data 

Public availability: A privacy setting that allows anyone to access a dashboard

Row-level permission: A privacy setting that controls the availability of specific rows of a table or dataset in a dashboard

Trade-off: Balancing various factors, often by prioritizing one element while sacrificing another, in order to arrive at the best possible result



# Review: DATA ANALYTICS CONTENT

## Aggregation

Welcome back.
In the next few videos, we'll explore something called data aggregation.
Aggregation means collecting or gathering many separate pieces into a whole,
for example, the Milky Way Galaxy is an aggregation of stars, dust, and gasses.
So, data aggregation is the process of gathering data from multiple
sources in order to combine it into a single summarized collection.
In data analytics, a summarized collection or summary describes
identifying the data you need and gathering it all together in one place.
For example, let's say you have a cabinet full of different puzzles, one day,
a shelf breaks and all the boxes topple over,
scattering the puzzle pieces everywhere.
To get each puzzle organized again,
you need to identify the pieces that correspond to each particular puzzle,
gather them together and put them back into their correct boxes,
only then can you work with these pieces and create a complete picture.
So in data,
the puzzle pieces represent the data that lives in different separate datasets.
Getting them organized is the aggregation process.
Then the piles of pieces that complete a single puzzle become your summary.
And finally,
putting those pieces back together is like analyzing them to gain important insights.
Data aggregation helps data analysts identify trends,
make comparisons, and gain insights that wouldn't be possible if each of
the data elements were analyzed on its own.
For instance, data on high school graduations for individual
students can be aggregated into a single graduation rate for an entire class.
Data can also be aggregated over a given time period to provide
statistics such as averages, minimums, maximums, and sums.
For example, that same yearly graduation rate data can be aggregated once again
into a summary that shows us graduation rates for districts, states and countries.
Here's another example, let's say you had data on real estate
sales in a particular neighborhood for each of the past ten years.
If you aggregated all of that data, you'd be able to discover the average price
of a home in that area and how values have increased or decreased over time.
Functions are a big help in making data aggregation possible.
You'll learn how to use some of the most common ones to create your summaries soon.
In addition, we'll talk about aggregating data using something called a subquery.
You've seen SQL in action, and you understand that a query is a request for
information from a database.
So a subquery, also called an inner or nested query,
is a query within another query.
After the next several videos, you'll know how to aggregate data and
understand the tools you'll be using along the way.
Let's get started. 


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
more movies about data analysts.
I'd watch that. But since
we can't watch a movie about data,
at least not yet, we'll do the next best thing.
Watch data about movies.
We're going to take a look at
this spreadsheet with movie data.
We know we can compare different movies and movie genres.
Turns out, you can do the same with
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
cast members are qualitative data.
Next up is quantitative data,
which can be measured or
counted and then expressed as a number.
This is data with a certain quantity, amount, or range.
In our spreadsheet here,
the last two columns show the movies budget,
and box office revenue.
The data in these columns is listed in dollars,
which can be counted,
so we know that data is quantitative.
We can go even deeper into quantitative data
and break it down into discrete or continuous data.
Let's check out discrete data first.
This is data that's counted
and has a limited number of values.
Going back to our spreadsheet,
we'll find each movies budget,
and box-office returns in columns M and
N. These are both examples of discrete data.
They can be counted and have a limited number of values.
For example, the amount of money
a movie makes can only be represented
with exactly two digits after
the decimal to represent cents.
There can't be anything between one and two cents.
Continuous data can be measured using a timer and
its value can be shown as a decimal with several places.
Let's imagine a movie about data analysts
that I'm definitely going to star in someday.
You could express that movie's run-time as
110.0356 minutes.
You could even add fractional data
after the decimal point if you needed to.
There's also nominal and ordinal data.
Nominal data is a type of
qualitative data that's categorized without a set order.
In other words, this data doesn't have a sequence.
Here's a quick example.
Let's say you're collecting data about movies.
You ask people if they've watched a given movie.
Their responses would be in the form of nominal data.
They could respond yes,
no, or not sure.
These choices don't have a particular order.
Ordinal data, on the other hand,
is a type of qualitative data with a set order or scale.
If you ask a group of people to rank a movie from 1-5,
some might rank it as a two,
others a four, and so on.
These rankings are in order of how
much each person liked the movie.
Now, let's talk about internal data,
which is data that lives within a company's own systems.
For example, if a movie studio had
compiled all of the data in the spreadsheet
using only their own collection methods
then it would be their internal data.
The great thing about internal data is that it's
usually more reliable and easier to collect.
But in this spreadsheet,
it's more likely that the movie studio
had to use data owned or shared
by other studios and
sources because it includes movies they didn't make.
That means they be collecting external data.
External data is, you guessed it,
data that lives and is
generated outside of an organization.
External data becomes particularly valuable when
your analysis depends on as many sources as possible.
A great thing about this data is that it's structured.
Structured data is data
that's organized in a certain format,
such as rows and columns,
spreadsheets and relational databases are
two examples of software
that can store data in a structured way.
You might remember our earlier exploration
of structured thinking,
which helps you add a framework to a problem so that
you can solve it in an organized and logical manner.
You can think of structured data in the same way.
Having a framework for the data makes the data
easily searchable and more analysis ready.
As a data analyst,
you'll work with a lot of structured data,
which will usually be in the form of a table,
spreadsheet or relational database.
But sometimes you'll come across unstructured data.
This is data that is not organized in
any easily identifiable manner.
Audio and video files are examples of unstructured data
because there's no clear way to
identify or organize their content.
Unstructured data might have internal structure,
but the data doesn't fit neatly in rows and
columns like structured data. There you have it.
Hopefully you're now more familiar with
data formats and how you might use them in your work,
and in just a bit,
you'll continue to explore a structured data and learn
even more about the data you'll
use most often as an analyst,
coming soon to a screen near you. 


## Tableau

Hello again.
We've already discussed how helpful data visualizations can be when we
want to fit a lot of knowledge into a small space.
Now it's time to explore.
A powerful tool that can help you create these visualizations and
bring your data to life.
It's called Tableau a visual analytics platform that makes it a lot easier to
explore and manage data.
You might remember hearing a bit about Tableau and
some of our earlier discussions but you're about to discover even more plus
when you get comfortable with Tableau you'll find it even easier to use similar
tools giving you another skill that will help you stand out in the job hunt
coming up will cover some of the features that make Tableau effective for
visualizations and why it's used across industries.
After that the fun really starts.
We'll jump right in and explore the Tableau interface, identifying and
applying the various tools it has to offer.
I'll show you how to add data sources, control visual elements and
work with a variety of features that will make your visualization really powerful
like any software platform, there's some best practices to keep in mind.
So I'll show you some examples of the good and
the bad when it comes to visualizations.
We'll also get creative using color vision deficiency palettes to make our
visualizations more accessible and we'll show you how multiple data sources can be
combined to tell a more comprehensive story.
By the time we wrap up here,
you'll be able to publish your own visualizations on Tableau.
I am so excited to lead you on this Tableau tour.
It's another useful tool that you'll be able to turn to as a future data analyst
so that you can visualize and publish data you care about.
After all, data has a story and this is your chance to share it with others.
Alright, let's discover what it's all about. 


## Dashboards

Have you ever been driving a car when one of
the warning lights on the dashboard suddenly comes on?
Maybe the gas gauge starts
blinking because you're getting low on fuel.
It's handy when you have
that alert right in front of you,
clearly showing you that you
need to pay attention to your gas level.
Can you imagine if cars didn't have dashboards?
We'd never know if we're about to run out of gas,
we'd have no idea if our tire pressure was
low or if it was time for an oil change.
Without dashboards,
if our car started acting differently,
we'd have to pull out the user manual,
sift through all that information inside,
and try to figure out the problem ourselves.
Car dashboards make it easy for
drivers to understand and respond to
any issues with their vehicles because they're
constantly tracking and analyzing the car status.
But as you've been learning,
dashboards aren't just for cars,
companies also use them to share information,
get people engage with business plans and goals,
and uncover potential problems.
Just like a car's dashboard,
data analytics dashboards take tons of
information and bring it to life in
a clear, visually interesting way.
This is extremely important
when telling a story with data,
which is why it's a big part of number 2
in our three-data storytelling steps.
You've learned that a dashboard is
a tool that organizes information from
multiple datasets into
one central location for tracking,
analysis, and simple visualization
through tables, charts, and graphs.
Dashboards do this by constantly
monitoring live incoming data.
As we've been discussing,
you can make dashboards that are specifically
designed to speak to your stakeholders.
You can think about who will be looking at the data,
and what they need from it,
and how often they'll use it.
Then you can make a dashboard with
the perfect information just for them.
This is helpful because people can get confused
and distracted when they're presented with too much data.
A dashboard keeps things neat
and tidy and easy to understand.
When designing a dashboard,
it's best to start simple with
just the most important data points.
If later on you discover something's missing,
you can always go back and tweak
your dashboard or create a new one.
An important part of dashboard design
is the placement or layout of your charts,
graphs, and other visuals.
These elements need to be cohesive,
which means they're balanced and make
good use of the space on the dashboard.
After you decide what information
should be on your dashboard,
you might need to re-size and reorganize
it so it works better for your users.
One option in Tableau is choosing
between a vertical or horizontal layout.
A vertical layout adjusts the height.
A horizontal layout resizes the width
of the views and objects it contains.
Also, as you can see here,
evenly distributing the items within your layout
helps create a clear and organized data visual.
You can select either tiled or floating layouts.
Tiled items are part of a single layer grid that
automatically resizes based on
the overall dashboard size.
Floating items can be layered over other objects.
In this example, the map and
scatterplots are tiled, they don't overlap.
This really helps make clear what the data is all about,
which is valuable because the majority of
people in the world are visual learners,
they process information based on what they see.
That's why sharing your dashboards with
stakeholders is such a valuable practice.
Now there's something important
to keep in mind about that:
sharing dashboards with others
likely means that you'll lose control of the narrative.
In other words, you won't be there to tell
the story of your data and share your key messages.
Dashboards put storytelling power
in the hands of the viewer.
That means they'll craft
their own narrative and draw their own conclusions.
But don't let that scare you away from
being collaborative and open.
Just understand the risks
that come with sharing your dashboards.
After all, sharing information and
resources means that you'll have more people
working on the solution to
a big problem or coming up with that next big idea.
This leads to more connections which can result
in really exciting new practices and innovations. 


## Effective data visualizations

A data visualization, sometimes referred to as a “data viz,” allows analysts to properly interpret data. A good way to think of data visualization is that it can be the difference between utter confusion and really grasping an issue. Creating effective data visualizations is a complex task; there is a lot of advice out there, and it can be difficult to grasp it all. In this reading, you are going to learn some tips and tricks for creating effective data visualizations. First, you'll review two frameworks that are useful for thinking about how you can organize the information in your visualization. Second, you'll explore pre-attentive attributes and how they can be used to affect the way people think about your visualizations. From there, you'll do a quick review of the design principles that you should keep in mind when creating your visualization. You will end the reading by reviewing some practices that you can use to avoid creating misleading or inaccurate visualizations. 

- Frameworks for organizing your thoughts about visualization

Frameworks can help you organize your thoughts about data visualization and give you a useful checklist to reference. Here are two frameworks that may be useful for you as you create your own data viz: 

1) The McCandless Method

You learned about the David McCandless method in the first lesson on effective data visualizations, but as a refresher, the McCandless Method lists four elements of good data visualization: 

    Information: the data you are working with
    Story: a clear and compelling narrative or concept
    Goal: a specific objective or function for the visual
    Visual form: an effective use of metaphor or visual expression

Note: One useful way of approaching this framework is to notice the parts of the graphic where there is incomplete overlap between all four elements. For example, visual form without a goal, story, or data could be a sketch or even art. Data plus visual form without a goal or function is eye candy. Data with a goal but no story or visual form is boring. All four elements need to be at work to create an effective visual.

2) Kaiser Fung’s Junk Charts Trifecta Checkup

This approach is a useful set of questions that can help consumers of data visualization critique what they are consuming and determine how effective it is. The Checkup has three questions:

    What is the practical question? 
    What does the data say?
    What does the visual say? 

Note: This checklist helps you think about your data viz from the perspective of your audience and decide if your visual is communicating your data effectively to them or not. In addition to these frameworks, there are some other building blocks that can help you construct your data visualizations. 

- Pre-attentive attributes: marks and channels

Creating effective visuals means leveraging what we know about how the brain works, and then using specific visual elements to communicate the information effectively. Pre-attentive attributes are the elements of a data visualization that people recognize automatically without conscious effort. The essential, basic building blocks that make visuals immediately understandable are called marks and channels. 

MARKS - Marks are basic visual objects like points, lines, and shapes. 

Every mark can be broken down into four qualities: 

1. Position - Where a specific mark is in space in relation to a scale or to other marks
	< simple line chart with two lines. One is red and one is blue, and there is obvious space between them. >

3. Size - How big, small, long, or tall a mark is
	< a plot with points that are different sizes >

4. Shape - Whether a specific object is given a shape that communicates something about it
	< horizontal bar chart, but bars are made of icons shaped like people >

5. Color - What color the mark is
	< a bar chart with a red, green, yellow, grey, and blue bar >

CHANNELS - Channels are visual aspects or variables that represent characteristics of the data. 

Channels are basically marks that have been used to visualize data. Channels will vary in terms of how effective they are at communicating data based on three elements: 

1. Accuracy - Are the channels helpful in accurately estimating the values being represented? 

	For example, color is very accurate when communicating categorical differences, like apples and oranges. 	But it is much less effective when distinguishing quantitative data like 5 from 5.5.
	< a plot with apples and oranges representing the data points >

2. Popout - How easy is it to distinguish certain values from others? 

	There are many ways of drawing attention to specific parts of a visual, and many of them leverage pre-attentive attributes like line length, size, line width, shape, enclosure, hue, and intensity.
	< a line chart with three blue lines and one red line >

3. Grouping - How good is a channel at communicating groups that exist in the data? 

	Consider the proximity, similarity, enclosure, connectedness, and continuity of the channel.
	< bar chart with four groups of bars. In each group, there is a red bar and a blue bar >

But, remember: the more you emphasize different things, the less that emphasis counts. The more you emphasize one single thing, the more that counts. 

- Design principles

Once you understand the pre-attentive attributes of data visualization, you can go on to design principles for creating effective visuals. These design principles are important to your work as a data analyst because they help you make sure that you are creating visualizations that communicate your data effectively to your audience. By keeping these rules in mind, you can plan and evaluate your data visualizations to decide if they are working for you and your goals. And, if they aren’t, you can adjust them! 

1. Choose the right visual: One of the first things you have to decide is which visual will be the most effective for your audience. Sometimes, a simple table is the best visualization. Other times, you need a more complex visualization to illustrate your point. 

2. Optimize the data-ink ratio: The data-ink entails focusing on the part of the visual that is essential to understanding the point of the chart. Try to minimize non-data ink like boxes around legends or shadows to optimize the data-ink ratio.

3. Use orientation effectively: Make sure the written components of the visual, like the labels on a bar chart, are easy to read. You can change the orientation of your visual to make it easier to read and understand. 

4. Color: There are a lot of important considerations when thinking about using color in your visuals. These include using color consciously and meaningfully, staying consistent throughout your visuals, being considerate of what colors mean to different people, and using inclusive color scales that make sense for everyone viewing them.

5. Numbers of things: Think about how many elements you include in any visual. If your visualization uses lines, try to plot five or fewer. If that isn’t possible, use color or hue to emphasize important lines. Also, when using visuals like pie charts, try to keep the number of segments to less than seven since too many elements can be distracting. 

6. Avoiding misleading or deceptive charts: A line graph with several colorful lines going in different directions. It is intentionally difficult to read.

As you are considering what kind of visualization to create and how to design it, you will want to be sure that you are not creating misleading or deceptive charts. As you have been learning, data analysis provides people with insights and knowledge they can use to make decisions. So, it is important that the visualizations you create are communicating your data accurately and truthfully. Here are some common errors to avoid so that your visualizations aren’t accidentally misleading: 

- What to avoid & Why

1. Cutting off the y-axis: Changing the scale on the y-axis can make the differences between different groups in your data seem more dramatic, even if the difference is actually quite small. 

2. Misleading use of a dual y-axis: Using a dual y-axis without clearly labeling it in your data visualization can create extremely misleading charts. 

3. Artificially limiting the scope of the data: If you only consider the part of the data that confirms your analysis, your visualizations will be misleading because they don’t take all of the data into account. 

4. Problematic choices in how data is binned or grouped: It is important to make sure that the way you are grouping data isn’t misleading or misrepresenting your data and disguising important trends and insights. 

5. Using part-to-whole visuals when the totals do not sum up appropriately: If you are using a part-to-whole visual like a pie chart to explain your data, the individual parts should add up to equal 100%. If they don’t, your data visualization will be misleading. 

6. Hiding trends in cumulative charts: Creating a cumulative chart can disguise more insightful trends by making the scale of the visualization too large to track any changes over time. 

7. Artificially smoothing trends: Adding smooth trend lines between points in a scatterplot can make it easier to read that plot, but replacing the points with just the line can actually make it appear that the point is more connected over time than it actually was. 


Finally, keep in mind that data visualization is an art form, and it takes time to develop these skills. Over your career as a data analyst, you will not only learn how to design good data visualizations, but you will also learn how to evaluate good data visualizations. Use these tips to think critically about data visualization—both as a creator and as an audience member.

- Further reading

1. The beauty of data visualization: In this video, David McCandless explains the need for design to not just be beautiful, but for it to be meaningful as well. Data visualization must be able to balance function and form for it to be relevant to your audience. 

2. ‘The McCandless Method’ of data presentation: At first glance, this blog appears to be written by a David McCandless fan, and it is. However, it contains very useful information and provides an in-depth look at the 5-step process that McCandless uses to present his data.

3. Information is beautiful: Founded by McCandless himself, this site serves as a hub of sample visualizations that make use of the McCandless method. Explore data from the news, science, the economy, and so much more and learn how to make visual decisions based on facts from all kinds of sources. 

4. Beautiful daily news: In this McCandless collection, explore uplifting trends and statistics that are beautifully visualized for your creative enjoyment. A new chart is released every day so be sure to visit often to absorb the amazing things happening all over the world.

5. The Wall Street Journal Guide to Information Graphics: The Dos and Don'ts of Presenting Data, Facts, and Figures: This is a comprehensive guide to data visualization, including chapters on basic data visualization principles and how to create useful data visualizations even when you find yourself in a tricky situation. This is a useful book to add to your data visualization library, and you can reference it over and over again. 


## Design thinking for visualization improvement

Design thinking for data visualization involves five phases:

    Empathize: Thinking about the emotions and needs of the target audience for the data visualization 

    Define: Figuring out exactly what your audience needs from the data

    Ideate: Generating ideas for data visualization

    Prototype: Putting visualizations together for testing and feedback

    Test: Showing prototype visualizations to people before stakeholders see them

As interactive dashboards become more popular for data visualization, new importance has been placed on efficiency and user-friendliness. In this reading, you will learn how design thinking can improve an interactive dashboard. As a junior analyst, you wouldn’t be expected to create an interactive dashboard on your own, but you can use design thinking to suggest ways that developers can improve data visualizations and dashboards.

- An example: online banking dashboard

Suppose you are an analyst at a bank that has just released a new dashboard in their online banking application. This section describes how you might explore this dashboard like a new user would, consider a user’s needs, and come up with ideas to improve data visualization in the dashboard. The dashboard in the banking application has the following data visualization elements:

1. Monthly spending is shown as a donut chart that reflects different categories like utilities, housing, transportation, education, and groceries. 

2. When customers set a budget for a category, the donut chart shows filled and unfilled portions in the same view.

3. Customers can also set an overall spending limit, and the dashboard will automatically assign the budgeted amounts (unfilled areas of the donut chart) to each category based on past spending trends.

This illustration shows a dashboard for online banking that has a donut chart to track spending versus budget.

- Empathize

First, empathize by putting yourself in the shoes of a customer who has a checking account with the bank. 

    Do the colors and labels make sense in the visualization? 
    How easy is it to set or change a budget? 
    When you click on a spending category in the donut chart, are the transactions in the category displayed?

What is the main purpose of the data visualization? If you answered that it was to help customers stay within budget or to save money, you are right! Saving money was a top customer need for the dashboard. 

- Define

Now, imagine that you are helping dashboard designers define other things that customers might want to achieve besides saving money. 

What other data visualizations might be needed? 

    Track income (in addition to spending)
    Track other spending that doesn’t neatly fit into the set categories (this is sometimes called discretionary spending)
    Pay off debt

Can you think of anything else?

- Ideate

Next, ideate additional features for the dashboard and share them with the software development team. 

    What new data visualizations would help customers?
    Would you recommend bar charts or line charts in addition to the standard donut chart?
    Would you recommend allowing users to create their own (custom) categories?

Can you think of anything else?

- Prototype

Finally, developers can prototype the next version of the dashboard with new and improved data visualizations. 

- Test

Developers can close the cycle by having you (and others) test the prototype before it is sent to stakeholders for review and approval.

- Key takeaways

This design thinking example showed how important it is to:

    Understand the needs of users
    Generate new ideas for data visualizations
    Make incremental improvements to data visualizations over time

You can refer to the following articles for more information about design thinking: 

1. Three Critical Aspects of Design Thinking for Big Data Solutions
2. Data and Design Thinking: Why Use Data in the Design Process?
