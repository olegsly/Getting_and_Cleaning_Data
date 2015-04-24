#CODEBOOK.md
#Course Project Code Book

The data for this project can be downloaded from: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

The R script, that was developed, named as run_analysis.R. It  contains the following steps:

1. Merging two sets (training and test) into one data set. 
	- Data set from ‘train/X_train.txt’ is merged with ‘test/X_test.txt’. The result is a 10299*561 data frame.
	- Data set from ‘train/subject_train.txt’ is merged with ‘test/subject_test.txt’. The result is a 10299*1 data frame with subject IDs, 
	- Data set from ‘train/y_train.txt’ is merged with ‘test/y_test.txt’. The result is also a 10299*1 data frame with activity IDs.

2. Reading ‘features.txt’ file and extracting only the measurements on the mean and standard deviation for each measurement. The result of this step is the data set with 66 indexes. Only 66 from 561 attributes from original data set are the measurements on the mean and standard deviation.

3. Reading file with labels ‘activity_labels.txt’ and applying descriptive activity names to name the activities in the data set. 

4. Labeling the data set with descriptive names. Converting to lower case, removing underscores and brackets. 

5. Storing the cleaned data to ‘merged_clean_data.txt’ file. 

6. Creating the second data set with the average of each measurement for each activity and each subject. The final result is stored as the file with name ‘averages.txt’. It is a 180*68 data frame. The first column is subject IDs, the second column is activity names,  the averages for each of the 66 attributes are in columns from 3 to 68.
