##-----------------------------------------------------------------------------------------
#**README**
##-----------------------------------------------------------------------------------------
#TITLE: Live Session Assignment Units 3 and 4. Creating projects in RStudio
##Project Abstract: Housing Sales Data Analysis - Brooklyn (Borough 3)
##Date Due: Thursday, June 2, 2016
##Contributors: Paola Leon, Ken Avery, Andrew Abbott, Earl Shaw
##-----------------------------------------------------------------------------------------
#**Table of Contents**
##1. Purpose
##2. Dependencies
##3. File Structure
##4. Implementation
##5. System Information
##-----------------------------------------------------------------------------------------
#***Purpose***
###The purpose of this project is to analyze housing sales data sets using RStudio with the results and associated files stored in a GitHub repository.
##-----------------------------------------------------------------------------------------
#***Dependencies***
### All analysis was performed using RStudio, version 0.99.896. 
### All documents are stored in a GitHub repository NAME:Livesession3Assignment   LOCATION: https://github.com/payolitec/Livesession3Assignment
### All housing data sets used in the project have come from Datasource: http://www1.nyc.gov/home/search/index.page?search-terms=Rolling+sales+update 
##-----------------------------------------------------------------------------------------
#***File Structure***
###1. README file:
NAME: README.md				LOCATION: https://github.com/payolitec/Livesession3Assignment/blob/master/README.md  
This file is located in the project root directory at https://github.com/payolitec/Livesession3Assignment. 
This file includes an explanation of the purpose of the project as well as dependencies, file structure and details regarding the project’s implementation.
###2. A Data directory: 
NAME: Data 				LOCATION: https://github.com/payolitec/Livesession3Assignment/blob/master/Data
This directory contains the following files: 
1) Raw file: 
NAME: rollingsales_queens.csv 		LOCATION: https://github.com/payolitec/Livesession3Assignment/blob/master/Data/rollingsales_queens.csv
2) Clean file:
NAME: rollingsales_queens2.csv		LOCATION: https://github.com/payolitec/Livesession3Assignment/blob/master/Data/rollingsales_queens2.csv
This file reconciles data issues such as data outliers, missing values, wrong data types and wrong data formats; normalizing data into the proper R classes.
3) Rollingsales_loadandclean.md LOCATION: https://github.com/payolitec/Livesession3Assignment/blob/master/Data/Rollingsales_loadandclean.md
This file contains R markdown code responsible for loading the raw data and cleaning it. For example, handling outliers, changing wrong data types, and normalized data into the proper R classes.
###3. An Analysis directory:
NAME: Analysis				            LOCATION: 
https://github.com/payolitec/Livesession3Assignment/tree/master/Analysis
This directory contains the following files:  
1) Homes data:
NAME:rollingsales_queenshomes.csv	LOCATION: https://github.com/payolitec/Livesession3Assignment/blob/master/Analysis/rollingsales_queenshomes.csv
2) Sales data:
NAME:rollingsales_queenssale.csv	LOCATION: https://github.com/payolitec/Livesession3Assignment/blob/master/Analysis/rollingsales_queenssale.csv
These files contain the exploratory data analysis performed over clean data to visualize and make comparisons (i) across neighborhoods, and (ii) across time.
3) Rollingsales_data_analysis.md* LOCATION: https://github.com/payolitec/Livesession3Assignment/blob/master/Analysis/Rollingsales_data_analysis.md
This file contains R markdown code responsible for loading the clean data and performing exploratory analysis on it, e.g. plots, histograms and summary statistics to determine any patterns and relationships among variables within the data set.
###4. A Paper directory:
NAME: Paper				                LOCATION: 
https://github.com/payolitec/Livesession3Assignment/tree/master/Paper
This directory contains the following files:
1) A txt file
NAME:Explanation.txt			        LOCATION: https://github.com/payolitec/Livesession3Assignment/blob/master/Paper/Explanation.txt
This file provides a summary of any patterns and/or relationships found within the cleaned data set.
2) A Microsoft Word file
NAME: LiveSessionAssignment Units 3 and 4 - Instructions	LOCATION:  https://github.com/payolitec/Livesession3Assignment/blob/master/Paper/LiveSessionAssignment%20Units%203%20and%204%20-%20Instructions.docx
This file contains the instructions for the Live Session Assignment Units 3 and 4
##-----------------------------------------------------------------------------------------
#***Implementation***
###The R code contained within the files will help analyze housing sales data and provide a path for discovering key patterns and trends capable of helping to provide insight into house sales in a particular locale.
##-----------------------------------------------------------------------------------------
#***System Iformation***
R version 3.2.5 (2016-04-14)
Platform: x86_64-w64-mingw32/x64 (64-bit)
Running under: Windows >= 8 x64 (build 9200)
 
locale:
[1] LC_COLLATE=English_United States.1252  LC_CTYPE=English_United States.1252   
[3] LC_MONETARY=English_United States.1252 LC_NUMERIC=C                          
[5] LC_TIME=English_United States.1252    
 
attached base packages:
[1] stats     graphics  grDevices utils     datasets  methods   base     
 
other attached packages:
[1] plyr_1.8.3
 
loaded via a namespace (and not attached):
[1] tools_3.2.5 Rcpp_0.12.4
##-----------------------------------------------------------------------------------------
