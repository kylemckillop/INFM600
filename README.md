# Data Set for Linking Maryland Crime and Poverty Rate, 2006 to 2013
#### University of Maryland, iSchool, INFM600 Information Discovery &amp; Analysis Project

-------
Version
-------

Version 1.0 (March 2016)

-----------
Description
-----------

We worked to combine two publically available Maryland data sets:
* __Crime by County__ Maryland county crime rates by year. Population is given for each county. (Maryland Statistical Analysis Center, 2016)
* __Poverty Rate__ Maryland county poverty rates and margin of error for the years 2006 to 2013. Data from the US Census Bureau was used to formulate these poverty rates. (Maryland Department of Planning, 2015)

By combining on county name and year, we have created a new table and database that can allow users to directly compare county poverty rates to crime rates for the years 2006 to 2013.


-----
Files
-----
* __/combined_files/__ 
    * __MarylandPovertyRateToCrimeRateDatabase.sql__ - Import of /individual_files/* for a MySQL database
    * __MarylandPovertyRateToCrimeRateFlatTable.csv__ - Join of /individual_files/* as one table for ease of use
* __/individual_files/__
    * __jurisdiction.csv__ - ID and name of the County
    * __poverty_rate.csv__ - ID of county from the jurisdiction.csv, and the associated rate of poverty and margin of error for the years 2006 to 2013
    * __violent_crime.csv__ - ID of county from the jurisdiction.csv, number of different types of crimes, their rate per 100k and percent change in their rate from the previous year for the years 1975 to 2014
* __/graphs/*__ - Folder containing plot graphs of initial findings with trend lines
* __README.txt__ - txt version of this markdown readme file
* __processing.txt__ - Steps taken to sanitize and combine original data into the format presented
 
-----------
What questions can be answered with this data set?
-----------
How does county poverty rate affect crime in Maryland? 

We hypothesize that a higher poverty rate increases crime rate, but is that true for all types of crime?

-----------
Initial Conclusions
-----------

| Crime per 100k | Correlation Coefficient | Graph |
|---|---|---|
|Breaking and Entering|0.59|[/graphs/poverty_to_breaking_and_entering.png](https://raw.githubusercontent.com/kylemckillop/INFM600/master/graphs/poverty_to_breaking_and_entering.png)|
|Murder|0.48| [/graphs/poverty_to_murder.png](https://raw.githubusercontent.com/kylemckillop/INFM600/master/graphs/poverty_to_murder.png) |
|Aggravated Assault|  0.43 | [/graphs/poverty_to_aggravated_assault.png](https://raw.githubusercontent.com/kylemckillop/INFM600/master/graphs/poverty_to_aggravated_assault.png)  |
|Violent Crime Rate|  0.41 | [/graphs/poverty_to_violent_crime_rate.png](https://raw.githubusercontent.com/kylemckillop/INFM600/master/graphs/poverty_to_violent_crime_rate.png)  |
|Rape| 0.40  |  [/graphs/poverty_to_rape.png](https://raw.githubusercontent.com/kylemckillop/INFM600/master/graphs/poverty_to_rape.png) |
|Overall Crime Rate| 0.36  | [/graphs/poverty_to_overall_crime_rate.png](https://raw.githubusercontent.com/kylemckillop/INFM600/master/graphs/poverty_to_overall_crime_rate.png)  |
|Property Crime Rate| 0.33  | [/graphs/poverty_to_property_crime_rate.png](https://raw.githubusercontent.com/kylemckillop/INFM600/master/graphs/poverty_to_property_crime_rate.png)  |
|Robbery| 0.31  | [/graphs/poverty_to_robbery.png](https://raw.githubusercontent.com/kylemckillop/INFM600/master/graphs/poverty_to_robbery.png)  |
|Larceny Theft | 0.23  | [/graphs/poverty_to_larceny_theft.png](https://raw.githubusercontent.com/kylemckillop/INFM600/master/graphs/poverty_to_larceny_theft.png)  |
| Motor Vehicle Theft  |  0.09 | [/graphs/poverty_to_motor_vehicle_theft.png](https://raw.githubusercontent.com/kylemckillop/INFM600/master/graphs/poverty_to_motor_vehicle_theft.png)  |

------- 
License
-------

The data in the INFM600 repository is distributed under a Creative Commons 
Attribution-NonCommercial-ShareAlike 4.0 International License (see 
http://creativecommons.org/licenses/by-nc-sa/4.0/).

----------
References
----------

Maryland Department of Planning. (2015, Nov 17). *Poverty Rate With Margin Of Error, 2006-2013* [Data set]. Retrieved from https://data.maryland.gov/Planning/Poverty-Rate-With-Margin-Of-Error-2006-2013/qnk2-m5pz

Maryland Statistical Analysis Center. (2016, Feb 08). *Violent Crime & Property Crime by County: 1975 to Present* [Data set]. Retrieved from https://data.maryland.gov/Public-Safety/Violent-Crime-Property-Crime-by-County-1975-to-Pre/jwfa-fdxs

-------
Credits
-------

   This dataset was built by Kyle McKillop and Neha Chanchlani.  To reference, you can use the following citation:
   
   McKillop, K., Chanchlani, N. (2016, March 17). *Data Set for Linking Maryland Crime and Poverty Rate, 2006 to 2013* [Data set]. Retrieved from https://github.com/kylemckillop/INFM600/
