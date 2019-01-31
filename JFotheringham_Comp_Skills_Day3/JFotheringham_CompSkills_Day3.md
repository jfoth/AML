>  **Title:** Analysis and Modelling Lab 
  **Subtitle:** General Computational Skills 
  **Project:** Day 3: Preparing Data For Analysis
  **Author:** Julia Fotheringham  
  **Affiliation:** University van Amsterdam
  >**Date:** January 30, 2019
**Resources:** 

Statistical abstract of the United States, 2012 (131st ed.). (2012). Section 6: Geography and the Environment. Washington, D.C.: U.S. Census Bureau. doi:https://www.census.gov/library/publications/2011/compendia/statab/131ed.html 


>**Software:**

 Data was processed in [openRefine](http://openrefine.org/) package
>**Data Resources:** 

The data table ["*391 - Highest and Lowest Temperatures by State Through 2003"*](https://www.census.gov/library/publications/2011/compendia/statab/131ed/geography-environment.html)  was sourced from [section 6: Geography and the Environment](https://www.census.gov/library/publications/2011/compendia/statab/131ed/geography-environment.html) of the [Resources: Statistical abstract of the United States, 2012 (131st ed.)](https://www.census.gov/library/publications/2011/compendia/statab/131ed.html)

>**Contents of Data Table:** 

The data table contains data relating to the highest and lowest recorded temperatures (<sup>o</sup>F) of each state in the United States of America. Data is sourced (non-consecutively) between 1885 and 2010. The temperature values are recorded as attributes of their State and include related information regarding the weather station where the recording was made, the date: *day, month, year* and annotations for max. and min. temperatures also recorded in other locations at earlier dates.

> **Data Preparation Process:** 

Order of processes	
 1. Use sort and facet to explore data and identify errors
	+ Facet> cluster> go through options to look for conflicts:
	+ “\1 Also on earlier dates at the same or other places.”
	+ Indentation removed by trim leading and tailing whitespace
	+ Use Text/Number Sort>Reverse to check if empty columns are empty before removing them

 2. Organise dates into three variable columns: day:month:year
	+ Sort and split into multiple columns based first on “,” to create a new column for “year” and then by “.” To separate the month.
	+ Use the “text filter” to cluster the date values marked with a “\1” (signifies a temperature extreme) and create a new variable column for the identifier.
	+ Delete superfluous columns created in the process
	+ Sort the month’s variable and use “edit” and “apply to all identical values” function to remove the “\1” from the notation
	+ To change the Months from text to numeric, code is available, however, there are only 12 possible variations, so sort and edit was used
	+ Adjust code to reflect to column identifiers and values and run again for the second date value.

 3. Empty rows/ repeated data
	+ The 1st row of data relates to the attributes for assets belonging to National extremes for the United States.  It is inconsistent with the other elements (they are based on States of the USA) and unnecessary to include as the data can be accessed via the “sort” function.
	+ Removed US max and min temperatures and the following empty row: starred rows to remove, facet by star, select starred rows, edit rows > remove all matching rows.

>**Script**

Script for all processes can be found at:
https://github.com/jfoth/AML/blob/master/JFotheringham_Comp_Skills_Day3/Cleaned_Min_Max_Temps_Script.rtf

> **Cleaned Data Table**

Cleaned data table (.csv) can be found at:
https://github.com/jfoth/AML/blob/master/JFotheringham_Comp_Skills_Day3/Cleaned_Min_Max_Temps-xls.csv