# data_cleaning-R
A workflow and exercises for data cleaning, processing, and munging tabular data in R
Data Cleaning and Organization
Data cleaning, processing, and munging can be a very time consuming processes. You can save time by developing a workflow for these tasks. Taking deliberate steps on the front end of your project to properly process your data will...

 help become familiar with your data and any quality issues that may exist, and

 save you from headaches down the road.

In this workshop I will present an outline that you can follow to help you with your day-to-day data organization tasks. Starting with a new, raw, tabular data set, we will follow these steps to learn more about it and clean up where we need to so we analyze it properly:

Data Cleaning (R Code):

1. Inital Exploration




         (i)   Data set dimensions (number of rows and columns)

         (ii)  Summary of variables

         (iii) Identify potential problems

         (iv)  Quick visualization
         
                       (a)Why visualize? Look at Anscombe’s quartet for an example.
         
                       (b)Observe outlying values
         
                       (c)Observe and understand the shape of the distributions

2.Fixing errors

         (i)Remove irrelevant columns or rows

         ii)Identify and deal with missing values

         iii)Look for and remove incorrect data (impossible values, duplicates, typos, and extra spaces)

         iv)Errors vs. Artifacts

3. Standardizing values
 
         i)Scaling
  
         ii)Normalization

4. Dimensionality reduction: Can you get rid of any columns?

         i)High ratio of missing values (based on a determined threshold)

         ii)High correlation with other variable(s)

5.Visualizing the cleaned data

6.Writing a cleaned data frame to a .csv file

7.Converting your df to a tibble (optional)

Data Dictionary 
This is usually a list of variables or data elements along with a description of each one (metadata about your data). You’ll want to include things like file name, column id, column name, variable type, count, notes, and warnings to your collaborators regarding any errors or mismatches. It's also a good idea to:

         
        i)Identify variable or columns as categorical, discrete numeric, or continuous
 
        ii)Get the overall dimensions of the data set (number of rows and columns)
        
       iii)Find out how many instances of each variable there are (total count)


You can create a data dictionary or codebook...

      i)Manually (e.g., in a spreadsheet)
      
     ii)Attach to your dataset (with the dataMeta package)

Data Exploration

     i)Descriptive Stats

    ii)Exploratory Data Analysis (EDA)

    iii)Visual presentation


Understanding data requires knowing the domain and the context


So that they are used properly, many of the techniques described above require that you understand the data. This means that you know the context in which the data were collected and have the domain knowledge to know if the data make sense. Making decisions on, for instance, how to normalize a certain variable in a data set without having a grasp on these two issues can results in data corruption or misrepresentation.
