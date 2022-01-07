# surfs_up
Using SQLite, SQAlchemy, Python in a Jupyter Notebook and Design a Flask application using data.

## Overview of Project

Surf n' Shake shop is a business idea opened in Oahu, Hawaii, to sell surfboards and ice cream to locals and tourists alike. An investor will be supporting this business, but it will be necessary to develop some analysis on a weather database to present information to improve this investor's decision-making, aiming at the business's success on this island. 

This assignment is related to the Bootcamp Data Analytics from the University of Toronto and comprises the goals below for this module: 

Follow below the goals for this module:

1) Objective 1: Determine the Summary Statistics for June
2) Objective 2: Determine the Summary Statistics for December

## Resources

* Data Files: [hawaii.sqlite](https://github.com/DougUOT/surfs_up/blob/main/hawaii.sqlite)
* Data Output: Data Source: [SurfsUp_Challenge.ipynb](https://github.com/DougUOT/surfs_up/blob/main/SurfsUp_Challenge.ipynb) 
* Software: Python 3.8.8, Anaconda 4.11.0, Jupyter Notebook 6.4.6, Pandas 1.3.4, Numpy 1.20.3, sqlalchemy 1.3.19, matplotlib 3.4.3 and Visual Studio Code 1.63.2

## Results

### Objective 1: Determine the Summary Statistics for June

Using Python, Pandas functions and methods, and SQLAlchemy, we will filter the date column of the Measurements table in the hawaii.sqlite database to retrieve all the temperatures for June. We will then convert those temperatures to a list, create a DataFrame from the list, and generate the summary statistics.

Import libraries (numpy, pandas, datetime, sqlalchemy) and an active query in writing to retrieve the June temperatures from the date column of the Measurement table: 

![](https://github.com/DougUOT/surfs_up/blob/main/Resouces/Surfsup_imag1.PNG)
![](https://github.com/DougUOT/surfs_up/blob/main/Resouces/Surfsup_imag2.PNG)

The temperatures are adding to a list:

![](https://github.com/DougUOT/surfs_up/blob/main/Resouces/Surfsup_imag3.PNG)

The list of temperatures is converting to a Pandas DataFrame, and Summary statistics are generating for the DataFrame:

![](https://github.com/DougUOT/surfs_up/blob/main/Resouces/Surfsup_imag4.PNG)


### Objective 2: Determine the Summary Statistics for December

Using Python, Pandas functions and methods, and SQLAlchemy, we will filter the date column of the Measurements table in the hawaii.sqlite database to retrieve all the temperatures for December. We will then convert those temperatures to a list, create a DataFrame from the list, and generate the summary statistics.

An active query is writing to retrieve the December temperatures from the date column of the Measurement table, and the temperatures are added to a list::

![](https://github.com/DougUOT/surfs_up/blob/main/Resouces/Surfsup_imag5.PNG)

The list of temperatures is converting to a Pandas DataFrame and summary statistics are generating for the DataFrame:

![](https://github.com/DougUOT/surfs_up/blob/main/Resouces/Surfsup_imag6.PNG)

## Summary

Based on the statistical results related to June and December, we have the results for Mean, Standard deviation, and for the 25%, 50% and 75% Percentiles, all very close, as summarized below: 

* Count: June 1700 and December 1517 | difference; 183 
* Mean: June, 74.94412 and December 71.041529 | difference; 3.902589 
* Std: June, 3.257417 and December 3.74592 | difference: 0.4885 
* Min: June, 64 and December 56 | difference; 8 
* 25%: June, 73 and December 69 | difference; 4 
* 50%: June, 75 and December 71 | difference; 4 
* 75%: June, 77 and December 74 | difference; 3 
* Max: June, 85 and December 83 | difference: 2 

### Follow below the three key differences in weather between June and December

First, the most significant difference found was about the minimum temperature in June with 64 and December with 56, a difference of 8 degrees Fahrenheit. Second, on the other hand, the minor difference is related to the Max, June with 85 and December with 83; we have only 2 degrees Fahrenheit. 

Last, the Standard deviation result comparing June and December was just 0.4885.

In short, based on the results obtained and data analysis, Oahu in Hawaii presents pleasant temperatures for surfing, considering with factor the very close results above, average temperature between 74.94 and 71.04 for June and December and the Max temperature extremely lovely on the island.

## Provide a two additional queries that would perform gather more weather data for June and December

### Query developed to retrieve the precipitation between 2010 and 2016 of June month:

According to ThoughtCo website: https://www.thoughtco.com/measuring-precipitation-1435346
* As according to the ThoughtCo website, Hawaii is an island in the United States and all precipitation is generally estimated in inches thinking about a 24-hour time frame, hypothetically, it is estimated thinking about that after downpour, for every an inch of rain that fell in a 24 hour term, we would have an inch of downpour on the floor.

![](https://github.com/DougUOT/surfs_up/blob/main/Resouces/Surfsup_imag7.PNG)
![](https://github.com/DougUOT/surfs_up/blob/main/Resouces/Surfsup_imag8.PNG)

The results show that the mean for the June month is around 0.158264 inches of rainfall.

### Query developed to retrieve the precipitation between 2010 and 2016 of December month

![](https://github.com/DougUOT/surfs_up/blob/main/Resouces/Surfsup_imag9.PNG)

The results show that the mean for the June month is around 0.169073 inches of rainfall.

### Query was developed to retrieve the temperature frequency in June and December 2016.

#### June of 2016

We considered the station USC00519281 with the highest observation in Hawaii; also, we considered the June month of 2016 as more recent data for this analysis.

![](https://github.com/DougUOT/surfs_up/blob/main/Resouces/Surfsup_imag10.PNG)

#### December of 2016

We considered the station USC00519281 with the highest observation in Hawaii; also, we considered the December month of 2016 as more recent data for this analysis.

![](https://github.com/DougUOT/surfs_up/blob/main/Resouces/Surfsup_imag11.PNG)

For both months (June and December of 2016), the results are very similar, with high concentrations on temperatures between 70 and 75 Fahrenheit.

## Recommendations for future Analysis

For future data analysis complementing this project, we suggest that other more recent databases search it. Other variables such as wind and temperature refer to the four seasons of the year that can influence the sales demand for ice cream or surfboards on the island.
