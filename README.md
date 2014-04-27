Getting-and-Cleaning-Data-Project
=================================


##Running the script
- Set your working directory
-	source("run_analysis.R")
-	Tidy dataset should be created in your current working directory as "Submit.txt"

##Assumptions
-	Data downloaded and extracted on your working directory https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 
-	Extracted folder renamed to "UCI_HAR_DATASET" 
-	 Test folder, train folder, "activity_labels.txt" and "features.txt" are available in "UCI_HAR_DATASET".

##Data transformation steps:
- The script creates two functions:
  - creatingTrain joins all the text files stored in the train folder and returns a data frame called Train
  - creatingTest joins all the text files stored in the test folder and returns a data frame called Test
- Then, run_analysis.R  joins both Train and Test in a data frame called "Final"
- Adds a new column called "Activity" and then fills this column with the activity labels based on each activity code.
- Reorder columns
- Gets all the columns related to means and standard deviations of the variables 
- Finally, the script rearranges the dataset as required and writes a new table called Submit.txt with 180 rows and 69 columns.

##Variables with mean and standard deviation (std) measurements:
- 1-	"Subject"
- 2-	"Activity"
- 3-	"Activity_Code"
- 4-	"tBodyAcc.mean.X"
- 5-	"tBodyAcc.mean.Y"
- 6-	"tBodyAcc.mean.Z"
- 7-	"tGravityAcc.mean.X"
- 8-	"tGravityAcc.mean.Y"
- 9-	"tGravityAcc.mean.Z"
- 10-	"tBodyAccJerk.mean.X"
- 11-	"tBodyAccJerk.mean.Y"
- 12-	"tBodyAccJerk.mean.Z"
- 13-	"tBodyGyro.mean.X"
- 14-	"tBodyGyro.mean.Y"
- 15-	"tBodyGyro.mean.Z"
- 16-	"tBodyGyroJerk.mean.X"
- 17-	"tBodyGyroJerk.mean.Y"
- 18-	"tBodyGyroJerk.mean.Z"
- 19-	"tBodyAccMag.mean"
- 20-	"tGravityAccMag.mean"
- 21-	"tBodyAccJerkMag.mean"
- 22-	"tBodyGyroMag.mean"
- 23-	"tBodyGyroJerkMag.mean"
- 24-	"fBodyAcc.mean.X"
- 25-	"fBodyAcc.mean.Y"
- 26-	"fBodyAcc.mean.Z"
- 27-	"fBodyAccJerk.mean.X"
- 28-	"fBodyAccJerk.mean.Y"
- 29-	"fBodyAccJerk.mean.Z"
- 30-	"fBodyGyro.mean.X"
- 31-	"fBodyGyro.mean.Y"
- 32-	"fBodyGyro.mean.Z"
- 33-	"fBodyAccMag.mean"
- 34-	"fBodyBodyAccJerkMag.mean"
- 35-	"fBodyBodyGyroMag.mean"
- 36-	"fBodyBodyGyroJerkMag.mean"
- 37-	"tBodyAcc.std.X"
- 38-	"tBodyAcc.std.Y"
- 39-	"tBodyAcc.std.Z"
- 40-	"tGravityAcc.std.X"
- 41-	"tGravityAcc.std.Y"
- 42-	"tGravityAcc.std.Z"
- 43-	"tBodyAccJerk.std.X"
- 44-	"tBodyAccJerk.std.Y"
- 45-	"tBodyAccJerk.std.Z"
- 46-	"tBodyGyro.std.X"
- 47-	"tBodyGyro.std.Y"
- 48-	"tBodyGyro.std.Z"
- 49-	"tBodyGyroJerk.std.X"
- 50-	"tBodyGyroJerk.std.Y"
- 51-	"tBodyGyroJerk.std.Z"
- 52-	"tBodyAccMag.std"
- 53-	"tGravityAccMag.std"
- 54-	"tBodyAccJerkMag.std"
- 55-	"tBodyGyroMag.std"
- 56-	"tBodyGyroJerkMag.std"
- 57-	"fBodyAcc.std.X"
- 58-	"fBodyAcc.std.Y"
- 59-	"fBodyAcc.std.Z"
- 60-	"fBodyAccJerk.std.X"
- 61-	"fBodyAccJerk.std.Y"
- 62-	"fBodyAccJerk.std.Z"
- 63-	"fBodyGyro.std.X"
- 64-	"fBodyGyro.std.Y"
- 65-	"fBodyGyro.std.Z"
- 66-	"fBodyAccMag.std"
- 67-	"fBodyBodyAccJerkMag.std"
- 68-	"fBodyBodyGyroMag.std"
- 69-	"fBodyBodyGyroJerkMag.std"
