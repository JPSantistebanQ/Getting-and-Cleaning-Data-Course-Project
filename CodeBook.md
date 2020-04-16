# Codebook

For information about how to dowload the data set used in this project go to the [README.md](https://github.com/JPSantistebanQ/Getting-and-Cleaning-Data-Course-Project/blob/master/README.md) file.

## Input files

The data set in folder 'UCI HAR Dataset' includes the following files:

* 'README.txt'
* 'features_info.txt': Shows information about the variables used on the feature vector.
* 'features.txt': List of all features.
* 'activity_labels.txt': Links the class labels with their activity name.
* 'train/X_train.txt': Training set.
* 'train/y_train.txt': Training labels.
* 'test/X_test.txt': Test set.
* 'test/y_test.txt': Test labels.

The following files are available for the train and test data. Their descriptions are equivalent. 

* 'train/subject_train.txt': Each row identifies the subject who performed the activity for each window sample. Its range is from 1 to 30. 

* 'train/Inertial Signals/total_acc_x_train.txt': The acceleration signal from the smartphone accelerometer X axis in standard gravity units 'g'. Every row shows a 128 element vector. The same description applies for the 'total_acc_x_train.txt' and 'total_acc_z_train.txt' files for the Y and Z axis. 

* 'train/Inertial Signals/body_acc_x_train.txt': The body acceleration signal obtained by subtracting the gravity from the total acceleration. 

* 'train/Inertial Signals/body_gyro_x_train.txt': The angular velocity vector measured by the gyroscope for each window sample. The units are radians/second. 

## The run_analysis script

The script created:

* Converts the raw data into R data frame objects
* Merges the train and test data into a single files for analysis
* Appends the subject ID to the appropriate row of data
* Changes the data column names to descriptive names
* Changes the activity data to descriptive names
* Produces an aggregated tidy data file of activities by subject

## Output

The final output is a tidy data set with the average of each variable for each activity and each subject and can be found [here](https://github.com/JPSantistebanQ/Getting-and-Cleaning-Data-Course-Project/blob/master/tidy_data.txt)

`secondDataSet` is the tidy data produced after going through all 5 steps of the course project. It contains 180 observations and 68 variables. Where the first column is the subject id, second column is the activity and the rest are the average of each feature variables.