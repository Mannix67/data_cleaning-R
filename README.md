# data_cleaning-R
A workflow and exercises for data cleaning, processing, and munging tabular data in R
Data Cleaning and Organization
Data cleaning, processing, and munging can be a very time consuming processes. You can save time by developing a workflow for these tasks. Taking deliberate steps on the front end of your project to properly process your data will...

help you become familiar with your data and any quality issues that may exist, and
save you from headaches down the road.
In this workshop we'll present an outline that you can follow to help you with your day-to-day data organization tasks. Starting with a new, raw, tabular data set, we will follow these steps to learn more about it and clean up where we need to so we analyze it properly:

Data Cleaning (R Code):
Inital Exploration
Data set dimensions (number of rows and columns)
Summary of variables
Identify potential problems
Quick visualization
Why visualize? Look at Anscombe’s quartet for an example.
Observe outlying values
Observe and understand the shape of the distributions
Fixing errors
Remove irrelevant columns or rows
Identify and deal with missing values
Look for and remove incorrect data (impossible values, duplicates, typos, and extra spaces)
Errors vs. Artifacts
Standardizing values
Scaling
Normalization
Dimensionality reduction: Can you get rid of any columns?
High ratio of missing values (based on a determined threshold)
High correlation with other variable(s)
Visualizing the cleaned data
Writing a cleaned data frame to a .csv file
Converting your df to a tibble (optional)
Data Dictionary (R Code)
This is usually a list of variables or data elements along with a description of each one (metadata about your data). You’ll want to include things like file name, column id, column name, variable type, count, notes, and warnings to your collaborators regarding any errors or mismatches. It's also a good idea to:

Identify variable or columns as categorical, discrete numeric, or continuous
Get the overall dimensions of the data set (number of rows and columns)
Find out how many instances of each variable there are (total count)
You can create a data dictionary or codebook...

Manually (e.g., in a spreadsheet)
Attach to your dataset (with the dataMeta package)
Data Exploration
Descriptive Stats
Exploratory Data Analysis (EDA)
Visual presentation
Understanding data requires knowing the domain and the context
So that they are used properly, many of the techniques described above require that you understand the data. This means that you know the context in which the data were collected and have the domain knowledge to know if the data make sense. Making decisions on, for instance, how to normalize a certain variable in a data set without having a grasp on these two issues can results in data corruption or misrepresentation.
