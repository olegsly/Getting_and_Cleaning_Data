#Getting_and_Cleaning_Data

#Getting and Cleaning Data Cource Project

- Unzip the source (https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip) into a folder on your local drive, ex. ‘~/R-projects/Getting_and_Cleaning_Data/Project/‘ 

*Please note. All paths a given for Mac OS X.*
- The folder ‘UCI HAR Dataset’ will be created in ‘~/R-projects/Getting_and_Cleaning_Data/Project/‘
- Put file run_analysis.R into ‘~/R-projects/Getting_and_Cleaning_Data/Project/UCI HAR Dataset’
- In RStudio run the command to setup your home directory, ex.: setwd(«~/R-projects/Getting_and_Cleaning_Data/Project/UCI HAR Dataset»)
- Then use source(«run_analysis.R») command
- Two new files would be created:

 -‘merged_clean_data.txt’ with data frame with 10299*68 dimension
 
 -‘averages.txt’ with data frame with 180*68 dimension

- Finally, use data <- read.table(«averages.txt») to read the data. 

It is 180x68 because there are 30 subjects and 6 activities, thus «for each activity and each subject» means 30 * 6 = 180 rows.
