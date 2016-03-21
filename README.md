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
* __Crime by County__ Maryland county crime rates by year. Population is given for each county  
* __Poverty Rate__ Maryland county poverty rates and margin of error for the years 2006 to 2013. Data from the US Census Bureau was used to formulate these poverty rates. (Maryland Department of Planning, 2015)




-----
Files
-----
* __/combined_files/__ 
    * __MarylandPovertyRateToCrimeRateDatabase.sql__ - Import of /individual_files/* for a MySQL database
    * __MarylandPovertyRateToCrimeRateFlatTable.csv__ - Join of /individual_files/* as one table for ease of use
* __/individual_files/__
    * __jurisdiction.csv__ - ID and name of the County.
    * __poverty_rate.csv__ - ID of the county from the above table, and the associated rate of poverty and Margin of Error for the years 2006 to 2013
    * __violent_crime.csv__ - ID of county from the jurisdiction.csv, number of different types of crimes, their rate per 100k and percent change in their rate from the previous year
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

TODO

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
   
   McKillop, K., Chanchlani, N. (2016, May 17). *Data Set for Linking Maryland Crime and Poverty Rate, 2006 to 2013* [Data set]. Retrieved from https://github.com/kylemckillop/INFM600/
