## Readme file regarding files associated with tidy data set containing Samsung activity data

### Introduction
This project concerns Samsung activity-monitoring data obtained from: 
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

Additional details about the data are available here:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

This project creates a tidy data set with the average for each subject and each activity of each measurement of the mean or standard deviation.  (More details appear below and in CodeBook.md.)

### Dataset
This project includes the following files:
*README.md

*run_analysis.R: creates a tidy data set, tidy.txt, with the average for each subject and each activity of each measurement of the mean or standard deviation (from the Samsung data); running this program requires having the Samsung data in the working directory (or following the commented instructions at the beginning of the file to download the data)

*tidy.txt: the tidy data set output by run_analysis.R

*CodeBook.md: describes the variables in tidy.txt

### About run_analysis.R

To use the script, you must have the Samsung data in your working directory (or follow the commented instructions at the beginning fo the file to download the data).  Typing source("run_analysis.R") and hitting <return> will produce the file tidy.txt

As explained in the comments in run_analysis.R, this script merges the training and test sets (from the Samsung data), extracts only measurements of the mean and standard deviation of each variable, assigns descriptive variable names, labels the activities with descriptive names, and creates a tidy data set, tidy.txt, with average of each variable for each activity and each subject

### About the raw Samsung data

This project uses Samsung activity-monitoring data obtained from: 
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

Additional details about the data are available here:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

The raw data sets concerns measurements of movement recorded by 30 subjects who were wearing a smartphone (a Samsung Galaxy S II).  Additional specific details about the measurements used to produce this raw data set are contained in the README.txt file for the Samsung data (available at the above url).

Specific information about the variables in tidy.txt is contained in CodeBook.md.  The section "About run_analysis.R" (above) describes how the Samsung data was manipuated.






