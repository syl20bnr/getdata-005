# Cookbook

The raw data used in this cookbook are available at the following address:
http://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

To get a description of the study, please visit the URL:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

## Transformations to clean the data
- The following files of the `train` data set have been `cbind` in this order:
  - `subject_train`
  - `Y_train`
  - `X_train`
- The following files of the `test` data set have been `cbind` in this order:
  - `subject_test`
  - `Y_test`
  - `X_test`
- The 2 resulting data frames have been `rbind`
- Only the columns for the means and the standard deviations have been kept
- the columns have been labeled:
  - SUBJECTS
  - ACTIVITIES
  - "BodyAccX_Mean",
  - "BodyAccY_Mean",
  - "BodyAccZ_Mean",
  - "BodyAccX_Std",
  - "BodyAccY_Std",
  - "BodyAccZ_Std",
  - "GravityAccX_Mean",
  - "GravityAccY_Mean",
  - "GravityAccZ_Mean",
  - "GravityAccX_Std",
  - "GravityAccY_Std",
  - "GravityAccZ_Std",
  - "BodyAccJerkX_Mean",
  - "BodyAccJerkY_Mean",
  - "BodyAccJerkZ_Mean",
  - "BodyAccJerkX_Std",
  - "BodyAccJerkY_Std",
  - "BodyAccJerkZ_Std",
  - "BodyGyroX_Mean",
  - "BodyGyroY_Mean",
  - "BodyGyroZ_Mean",
  - "BodyGyroX_Std",
  - "BodyGyroY_Std",
  - "BodyGyroZ_Std",
  - "BodyGyroJerkX_Mean",
  - "BodyGyroJerkY_Mean",
  - "BodyGyroJerkZ_Mean",
  - "BodyGyroJerkX_Std",
  - "BodyGyroJerkY_Std",
  - "BodyGyroJerkZ_Std",
  - "BodyAccMag_Mean",
  - "BodyAccMag_Std",
  - "GravityAccMag_Mean",
  - "GravityAccMag_Std",
  - "BodyAccJerkMag_Mean",
  - "BodyAccJerkMag_Std",
  - "BodyGyroMag_Mean",
  - "BodyGyroMag_Std",
  - "BodyGyroJerkMag_Mean",
  - "BodyGyroJerkMag_Std",
  - "BodyAccX_Mean",
  - "BodyAccY_Mean",
  - "BodyAccZ_Mean",
  - "BodyAccX_Std",
  - "BodyAccY_Std",
  - "BodyAccZ_Std",
  - "BodyAccJerkX_Mean",
  - "BodyAccJerkY_Mean",
  - "BodyAccJerkZ_Mean",
  - "BodyAccJerkX_Std",
  - "BodyAccJerkY_Std",
  - "BodyAccJerkZ_Std",
  - "BodyGyroX_Mean",
  - "BodyGyroY_Mean",
  - "BodyGyroZ_Mean",
  - "BodyGyroX_Std",
  - "BodyGyroY_Std",
  - "BodyGyroZ_Std",
  - "BodyAccMag_Mean",
  - "BodyAccMag_Std",
  - "BodyAccJerkMag_Mean",
  - "BodyAccJerkMag_Std",
  - "BodyGyroMag_Mean",
  - "BodyGyroMag_Std",
  - "BodyGyroJerkMag_Mean",
  - "BodyGyroJerkMag_Std")

## Tidy data set with average values
See the [README.md](https://github.com/syl20bnr/getdata-005/blob/master/README.md)
file in order to create this data set.

The data set is stored in the file `"avg_tidy_dataset_getdata-005.txt"`.

This data represent the average of the means and standard deviations of each
variable for each (subject, activity) pair.

The first column is the subject, the second is the activity, the subsequent
columns are the average of the means and standard deviations.

The number of subject is `30` and the activities are:
- WALKING
- WALKING_UPSTAIRS
- WALKING_DOWNSTAIRS
- SITTING
- STANDING
- LAYING

The columns labels are the same as the cleaned data.
