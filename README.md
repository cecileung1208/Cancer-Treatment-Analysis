# Cancer Treatment Analysis

![Image](https://news.usc.edu/files/2018/03/Nanoparticle-cancer-detection-web.jpg)

## Background

The goal of this analysis is to determine the effectiveness of the 10 difference cancer drug treatments results being tested on 248 mice over the course of 45 days.  Results of the mice results have been provided in CSV datasets.  Python with Pandas, Numpy, and Matplotlib (through Jupyter Notebooks) was used to clean and process the data, as well as calculate and display the desired outputs.

## Dataset

*    [Mouse Metadata](https://github.com/cecileung1208/Matplotlib-The-Power-of-Plots/blob/master/Pymaceuticals/data/Mouse_metadata.csv)<br>
*    [Study Results](https://github.com/cecileung1208/Matplotlib-The-Power-of-Plots/blob/master/Pymaceuticals/data/Study_results.csv)

## Requirement

1. Import dependencies
2. Import the csv datasets
3. Creating Dataframe
   * Merge datasets into Jupyter notebook.
   * Check the number of unique mouse IDs.
   * Determine if there are any duplicates mouse ID and time points.  If so, drop those values.
4. Generate a summary statistics table of mean, median, variance, standard deviation, and SEM of the tumor volume for each regimen by the following methods:
   * Groupby and Summary
   * Aggregate
5. Create a bar chart showing total number of mice tested against the 10 drug regimen using the following methods:
   *   Pandas
   *   Pyplot
6. Create a pie chart showing the gender distribution of all the mice using the following methods:
   *   Pandas
   *   Pyplot
7. Create a box plot graph to calculate the final size of the tumor across the 4 drug regimen, Capomulin, Ramicane, Infubinol, and Ceftamin.
   *   Merge this group df with the original dataframe to get the tumor volume at the last timepoint and filter for the 4 drug regimen.
   *   Create list for treatment names and tumor volumes.
   *   Calculate the quartiles, interquartiles range, upper and lower bounds across the 4 drug regimen.
   *   Create a list of the tumor sizes against the drug regimen.
   *   Determine outliers using upper and lower bounds across the drug regimen.
   *   Plot the boxes and outliers across the 4 drug regimen.
8. Create a line graph tumor volume vs time point of a specific mouse under the Capomulin drug regimen.
9. Create a scatter plot of tumor volume vs weight of all mouses under the Capomulin drug regimen.
   *   Filter for Capomulin.
   *   Group by drug regimen and get the mean of the tumor volume.
   *   Plot the scatter plot.
10. Calculate the correlation coefficient and linear regression model and plot the line against the scatter plot.

## Results


**1. Even Sample Size and Gender Distribution to ensure consistency in results.**

* From the bar graph, there are approximately 25 mice for each of the ten drug regimens.
![Image](https://github.com/cecileung1208/Cancer-Treatment-Analysis/blob/master/Pymaceuticals/Images/bar.png)

* From the pie chart, there is almost a 50% distribution amongst the male and female mice.
![Image](https://github.com/cecileung1208/Cancer-Treatment-Analysis/blob/master/Pymaceuticals/Images/pie.png)

**2.	Capomulin and Ramicane are the most effective drugs in reducing the tumor size.**
*    All mice had a tumor size of 45 mm3 on Day 0.
* 	 Based on the box plot diagram, some of the mice tumor size reduced to approximately 25mm3 and 22mm3 for Capomulin and     
     Ramicane respectively.
     
![Image](https://github.com/cecileung1208/Cancer-Treatment-Analysis/blob/master/Pymaceuticals/Images/boxplot.png)

**3.	The tumor volume decreases over the 45 days of take the Capomulin drug.**
![Image](https://github.com/cecileung1208/Cancer-Treatment-Analysis/blob/master/Pymaceuticals/Images/line.png)

**4.	There is a positive correlation between the tumor size and weight for Capomulin.**
* 	The correlation coefficient is 0.84 which shows when the weight increases, the tumor size increases too.
![Image](https://github.com/cecileung1208/Cancer-Treatment-Analysis/blob/master/Pymaceuticals/Images/scatter.png)
