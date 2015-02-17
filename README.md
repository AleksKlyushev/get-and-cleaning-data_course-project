# Getting And Cleaning Data - Course Project

## Introduction

This repo contains my course project to [Coursera](https://www.coursera.org) ["Getting And Cleaning Data"](https://class.coursera.org/getdata-002) course that is part of [Data Science](https://www.coursera.org/specialization/jhudatascience/1?utm_medium=listingPage) specialization.

There is just one script called `run_analysis.R`. It tries to accomplish all the 5 tasks mentioned in the instructions.

1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement. 
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive variable names. 
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
    
The code "Prints" out the task numbers as they are being processed. This visual feedback was found necessary to ensure that the processing had not stalled. 


The `CodeBook.md` explains the final output in more detailed.


## Run from command line

1. Clone this repo in your working directory using the following command:

        git clone https://github.com/ashwingrao/get-and-cleaning-data_course-project.git
       
2. Run the script (this assumes that you have installed "R" already):

        $ Rscript run_analysis.R
       
      - If the progream errors out, please make sure that the "UCI HAR Dataset" data is in the same folder. This data can be downloaded from: 
      https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip . Once you download, please change  
      your directory into this folder before running the script.
      You will get the following output:
      
          Prompt within UCI HAR Dataset folder> Rscript run_analysis.R 
            [1] "Performing Task 1..."
            [1] "Performing Task 4..."
            [1] "Performing Task 3..."
            [1] "Performing Task 2..."
            [1] "Performing Task 5..."
            [1] "Generating 'tidyset.txt' file"
           Prompt within UCI HAR Dataset folder>


3. Look for the final dataset named "tidyset.txt" file in the same directory and view the file (the command shows first three rows)

	       $ head -3 tidyset.txt
	   

