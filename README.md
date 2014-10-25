# Cleaning_and_Getting_Data

## Introduction to "run_analysis.R"
- 1) Merges the training and the test sets to create one data set.
- 2) Extracts only the measurements on the mean and standard deviation for each measurement.
- 3) Uses descriptive activity names to name the activities in the data set
- 4) Appropriately labels the data set with descriptive activity names.
- 5) Creates a second, independent tidy data set with the average of each variable for each activity and each subject.
 
## How to Run
- 1) Download the data source from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
- 2) Unzip the data set into your current working directory and you will see a folder UCI HAR Dataset
- 3) Run the R script (run_analysis.R) from the folder that contains UCI HAR Dataset
- 4) Two output files are generated in the current working directory. 
    - a) tidy_mean.txt: tidy data set with the average of each variable for each activity and each subject
    - b) tidy.txt: tidy data set

## Dependencies
The R script assumes you have 'data.table' installed using install.packages("data.table") and 'reshape2' installed using install.packages("reshape2").
