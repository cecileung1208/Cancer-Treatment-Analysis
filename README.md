# Cancer Treatment Analysis

![Image](https://news.usc.edu/files/2018/03/Nanoparticle-cancer-detection-web.jpg)

## Background

The goal of this analysis is to determine the effectiveness of the 10 difference cancer drug treatments results being tested on 248 mice over the course of 45 days.  Results of the mice results have been provided in CSV datasets.  Python with Pandas, Numpy, and Matplotlib (through Jupyter Notebooks) was used to clean and process the data, as well as calculate and display the desired outputs.

## Dataset

*    [Mouse Metadata](https://github.com/cecileung1208/Matplotlib-The-Power-of-Plots/blob/master/Pymaceuticals/data/Mouse_metadata.csv)<br>
*    [Study Results](https://github.com/cecileung1208/Matplotlib-The-Power-of-Plots/blob/master/Pymaceuticals/data/Study_results.csv)

## Requirement

* Import dependencies.
* Creating Dataframe
  * Import and merge datasets into Jupyter notebook.
  * Check the number of unique mouse IDs.
  * Determine if there are any duplicates mouse ID and time points.  If so, drop those values.
* Generate a summary statistics table of mean, median, variance, standard deviation, and SEM of the tumor volume for each regimen by the following methods:
  * Groupby and Summary
  * Aggregate
* Create a bar chart showing total number of mice tested against the 10 drug regimen using the following methods:
  *   Pandas
  *   Pyplot
* Create a pie chart showing the gender distribution of all the mice using the following methods:
  *   Pandas
  *   Pyplot
* Create a box plot graph to calculate the final size of the tumor across the 4 drug regimen, Capomulin, Ramicane, Infubinol, and Ceftamin.
  *   Merge this group df with the original dataframe to get the tumor volume at the last timepoint and filter for the 4 drug regimen.
  *   Create list for treatment names and tumor volumes.
  *   Calculate the quartiles, interquartiles range, upper and lower bounds across the 4 drug regimen.
  *   Create a list of the tumor sizes against the drug regimen.
  *   Determine outliers using upper and lower bounds across the drug regimen.
  *   Plot the boxes and outliers across the 4 drug regimen.
* Create a line graph tumor volume vs time point of a specific mouse under the Capomulin drug regimen.
* Create a scatter plot of tumor volume vs weight of all mouses under the Capomulin drug regimen.
  *   Filter for Capomulin.
  *   Group by drug regimen and get the mean of the tumor volume.
  *   Plot the scatter plot.
 * Calculate the correlation coefficient and linear regression model and plot the line against the scatter plot.

## Results



As a Senior Data Analyst at Pymaceuticals, I have generated tables and figures from the given information on the results of 10 different drug treatments for squamous cell carcinoma (SCC), a commonly occuring form of skin scancer.  248 mice identified with SCC tumor were evenly tested across different drug regimens in a course of 45 days to determine if the tumor size have decreased.

## **The Summary of Results have the following outputs:**

### **Pymaceuticals - Jupyter Notebook**

This [file](https://github.com/cecileung1208/Matplotlib-The-Power-of-Plots/blob/master/Pymaceuticals/Pymaceuticals.ipynb) provides program codes that output various graphs and tables that determine the results of the cancer treatments across different drug regimen for 248 mice.  

**The output are as follows:**
*    Observations and Insights

**Summary Statistics of Tumor Volume by Drug Regimen**

The mean, median, variance, standard deviation, and standard error from mean (sem) of the tumor volume will be calculated across the 10 drug regimen by the :
*    Groupby Method
*    Aggregate Method

**Bar Graph of Unique Mice by Drug Regimen**
*   Dataframe Panda Method
*   Pyplot Method

**Pie Chart of Mice Gender Distribution**
*    Dataframe Panda Method
*    Pyplot Method

**Quartiles, Interquartiles and Boxplot of Most Promising Drug Regimen**

The 4 drug regimens are: Capomulin, Ceftamin, Infubinol, Ramicane
*    Quartiles and Interquartiles Results of the 4 Most Promising Drug Regimen
*    Outliers of the 4 Most Promising Drug Regimen
*    Boxplot of the 4 Most Promising Drug Regimen

**Line Graph of Tumor Size vs Timepoint**
*    Results for a Specific Mouse under the Capomulin Drug Regimen

**Scatter Plot of Average Tumor Size vs Weight**
*    Results under the  Capomulin Drug Regimen

**Coeeficient Correlation and Linear Regression Model of Average Tumor Size vs Weight** 
*    Results of Coefficient Correlation and Linear Regression under the Capomulin Scatter Plot

### **2.  Pymaceuticals Data Source**

The data frame is extracted from the following CSV Files in the [data directory](https://github.com/cecileung1208/Matplotlib-The-Power-of-Plots/tree/master/Pymaceuticals/data):
*    [Mouse Metadata](https://github.com/cecileung1208/Matplotlib-The-Power-of-Plots/blob/master/Pymaceuticals/data/Mouse_metadata.csv)
*    [Study Results](https://github.com/cecileung1208/Matplotlib-The-Power-of-Plots/blob/master/Pymaceuticals/data/Study_results.csv)
