# Module_5_Challenge
Instructions
This assignment is broken down into the following tasks:

Prepare the data.

Generate summary statistics.

Create bar charts and pie charts.

Calculate quartiles, find outliers, and create a box plot.

Create a line plot and a scatter plot.

Calculate correlation and regression.

Submit your final analysis.

Prepare the Data
Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.

Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.

Display the updated number of unique mice IDs.

Generate Summary Statistics
Create a DataFrame of summary statistics. Remember, there is more than one method to produce the results you're after, so the method you use is less important than the result.

Your summary statistics should include:

A row for each drug regimen. These regimen names should be contained in the index column.

A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

Create Bar Charts and Pie Charts
Generate two bar charts. Both charts should be identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.

Create the first bar chart with the Pandas DataFrame.plot() method.

Create the second bar chart with Matplotlib's pyplot methods.

Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

Create the first pie chart with the Pandas DataFrame.plot() method.

Create the second pie chart with Matplotlib's pyplot methods.

Calculate Quartiles, Find Outliers, and Create a Box Plot
Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:

Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.

Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.

Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.

Determine outliers by using the upper and lower bounds, and then print the results.

Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.

hint: All four box plots should be within the same figure. Use this Matplotlib documentation pageLinks to an external site. for help with changing the style of the outliers.

Create a Line Plot and a Scatter Plot
Select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.

Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

Calculate Correlation and Regression
Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.

Plot the linear regression model on top of the previous scatter plot.

Requirements
Prepare the Data 
The datasets are merged into a single DataFrame. 
The number of mice are shown from the merged DataFrame. 
Each duplicate mice is found based on the Mouse ID and Timepoint. 
A clean DataFrame is created with the dropped duplicate mice. 
The number of mice are shown from the clean DataFrame. 
Generate Summary Statistics (15 points)
The mean of the tumor volume for each regimen is calculated using groupby. 
The media of the tumor volume for each regimen is calculated using groupby. 
The variance of the tumor volume for each regimen is calculated using groupby. 
The standard deviation of the tumor volume for each regimen is calculated using groupby. 
The SEM of the tumor volume for each regimen is calculated using groupby. 
A new DataFrame is created with using the summary statistics. 
Create Bar Charts and Pie Charts 
A bar plot showing the total number of timepoints for all mice tested for each drug regimen using Pandas is generated. 
A bar plot showing the total number of timepoints for all mice tested for each drug regimen using pyplot is generated.
A pie plot showing the distribution of female versus male mice using Pandas is generated. 
A pie plot showing the distribution of female versus male mice using pyplot is generated. 
Calculate Quartiles, Find Outliers, and Create a Box Plot 
A DatFrame that has the last timepoint for each mouse ID is created using groupby. 
The index of the DataFrame is reset. 
Retrieve the maximum timepoint for each mouse. 
The four treatment groups, Capomulin, Ramicane, Infubinol, and Ceftamin, are put in a list. 
An empty list is created to fill with tumor volume data. 
A for loop is used to display the interquartile range (IQR) and the outliers for each treatment group 
A box plot is generated that shows the distribution of the final tumor volume for all the mice in each treatment group. 
Create a Line Plot and a Scatter Plot 
A line plot is generated that shows the tumor volume vs. time point for one mouse treated with Capomulin. 
A scatter plot is generated that shows average tumor volume vs. mouse weight for the Capomulin regimen. 
Calculate Correlation and Regression 
The correlation coefficient and linear regression model are calculated for mouse weight and average tumor volume for the Capomulin regimen. 
