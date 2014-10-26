Getting-and-Cleaning-Data
=========================

Data Science specialization stream from Johns Hopkins (online via Coursera)

Getting and Cleaning Data
Course Project
We have to access data from the UCI, Machine Learning repository at https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

Transformation details
We have to merge two datasets into one and clean this dataset. Eventually, we have to create one R script called ‘run_analysis.r’ that does the following.
1.	Merges the training and the test sets to create one data set.
2.	Extracts only the measurements on the mean and standard deviation for each measurement.
3.	Uses descriptive activity names to name the activities in the data set
4.	Appropriately labels the data set with descriptive activity names.
5.	Creates a second, independent tidy data set with the average of each variable for each activity and each subject.
Steps to work through creating a tidy dataset
1.	Download the data source and put into a folder on your local drive. You'll have a UCI HAR Dataset folder.
2.	Put run_analysis.R in the parent folder of UCI HAR Dataset, then set it as your working directory using setwd()function in RStudio.
3.	Run source("run_analysis.R"), to generate a new file tiny_data.txt in the working directory.
Dependencies
run_analysis.R file will help install the dependencies automatically. It depends on reshape2 and data.table.
How run_analysis.R implements the above steps:
•	Load both test and train data
•	Load the features and activity labels.
•	Extract the mean & standard deviation column names & data.
•	Process the data. There are two parts processing test and train data respectively.
•	Merge data set.

