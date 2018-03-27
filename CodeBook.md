Peer-graded Assignment: Getting and Cleaning Data Course Project
By: Cecilia Cruz-Ram, MD

CodeBook.md

This file describes the variables, the data, and any transformations or work that were performed to clean up the data.

The data for the project:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

##Variable and descriptions ###Subject The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years.

Variable name	  Description
subject	        ID of the 30 volunteers who performed the activity. Its range is from 1 to 30.

###Activity Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist.

Variable name	  Description
activity	      Activity type that the 30 volunteers who performed the activity.
             |  Its has 6 levels:
             |   1. WALKING
             |   2. WALKING_UPSTAIRS
             |   3. WALKING_DOWNSTAIRS
             |   4. SITTING
             |   5. STANDING
             |   6. LAYING
             
###Features Using its embedded accelerometer and gyroscope, 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz are captured. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.

The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals timeAccelerometer a-XYZ and timeGyroscope-XYZ. These time domain signals were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (timeBodyacceleration-XYZ and timeGravityAcceleration-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz.

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (timeBodyAccelerationJerk-XYZ and timeBodyGyroscopeJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (timeBodyAccelerationMagnitude, timeGravityAccelerationMagnitude, timeBodyAccelerationJerkMagnitude, timeBodyGyroscopeMagnitude, timeBodyGyroscopeJerkMagnitude).

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcceleration-XYZ, frequencyBodyAccelerationJerk-XYZ, frequencyBodyGyro-XYZ, frequencyBodyAccelerationJerkMagnitude, frequencyBodyGyroMagnitude, frequencyBodyGyroJerkMagnitude.

These signals were used to estimate variables of the feature vector for each pattern:
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

o timeBodyAccelerometer-XYZ
o timeGravityAccelerometer-XYZ
o timeBodyAccelerometerJerk-XYZ
o timeBodyGyroscope-XYZ
o timeBodyGyroscopeJerk-XYZ
o timeBodyAccelerometerMagnitude
o timeGravityAccelerometerMagnitude
o timeBodyAccelerometerJerkMagnitude
o timeBodyGyroscopeMagnitude
o timeBodyGyroscopeJerkMagnitude
o frequencyBodyAccelerometer-XYZ
o frequencyBodyAccelerometerJerk-XYZ
o frequencyBodyGyroscope-XYZ
o frequencyBodyAccelerometerMagnitude
o frequencyBodyAccelerometerJerkMagnitude
o frequencyBodyGyroscopeMagnitude
o frequencyBodyGyroscopeJerkMagnitude

The set of variables that were estimated from these signals are:

o mean(): Mean value
o std(): Standard deviation

Identifiers

o subject - The ID of the test subject
o activity - The type of activity performed when the corresponding measurements were taken

Tidy Data Structure

###Column Heading (Unit wise)

o timeBodyAccelerometer-mean()-X (radians per sec)
o timeBodyAccelerometer-mean()-Y (radians per sec)
o timeBodyAccelerometer-mean()-Z (radians per sec)
o timeBodyAccelerometer-std()-X (radians per sec)
o timeBodyAccelerometer-std()-Y (radians per sec)
o timeBodyAccelerometer-std()-Z (radians per sec)
o timeGravityAccelerometer-mean()-X (radians per sec)
o timeGravityAccelerometer-mean()-Y (radians per sec)
o timeGravityAccelerometer-mean()-Z (radians per sec)
o timeGravityAccelerometer-std()-X (radians per sec)
o timeGravityAccelerometer-std()-Y (radians per sec)
o timeGravityAccelerometer-std()-Z (radians per sec)
o timeBodyAccelerometerJerk-mean()-X (radians per sec)
o timeBodyAccelerometerJerk-mean()-Y (radians per sec)
o timeBodyAccelerometerJerk-mean()-Z (radians per sec)
o timeBodyAccelerometerJerk-std()-X (radians per sec)
o timeBodyAccelerometerJerk-std()-Y (radians per sec)
o timeBodyAccelerometerJerk-std()-Z (radians per sec)
o timeBodyGyroscope-mean()-X (radians per sec)
o timeBodyGyroscope-mean()-Y (radians per sec)
o timeBodyGyroscope-mean()-Z (radians per sec)
o timeBodyGyroscope-std()-X (radians per sec)
o timeBodyGyroscope-std()-Y (radians per sec)
o timeBodyGyroscope-std()-Z (radians per sec)
o timeBodyGyroscopeJerk-mean()-X (radians per sec)
o timeBodyGyroscopeJerk-mean()-Y (radians per sec)
o timeBodyGyroscopeJerk-mean()-Z (radians per sec)
o timeBodyGyroscopeJerk-std()-X (radians per sec)
o timeBodyGyroscopeJerk-std()-Y (radians per sec)
o timeBodyGyroscopeJerk-std()-Z (radians per sec)
o timeBodyAccelerometerMagnitude-mean() (radians per sec)
o timeBodyAccelerometerMagnitude-std() (radians per sec)
o timeGravityAccelerometerMagnitude-mean() (radians per sec)
o timeGravityAccelerometerMagnitude-std() (radians per sec)
o timeBodyAccelerometerJerkMagnitude-mean() (radians per sec)
o timeBodyAccelerometerJerkMagnitude-std() (radians per sec)
o timeBodyGyroscopeMagnitude-mean() (radians per sec)
o timeBodyGyroscopeMagnitude-std() (radians per sec)
o timeBodyGyroscopeJerkMagnitude-mean() (radians per sec)
o timeBodyGyroscopeJerkMagnitude-std() (radians per sec)
o frequencyBodyAccelerometer-mean()-X (hertz)
o frequencyBodyAccelerometer-mean()-Y (hertz)
o frequencyBodyAccelerometer-mean()-Z (hertz)
o frequencyBodyAccelerometer-std()-X (hertz)
o frequencyBodyAccelerometer-std()-Y (hertz)
o frequencyBodyAccelerometer-std()-Z (hertz)
o frequencyBodyAccelerometerJerk-mean()-X (hertz)
o frequencyBodyAccelerometerJerk-mean()-Y (hertz)
o frequencyBodyAccelerometerJerk-mean()-Z (hertz)
o frequencyBodyAccelerometerJerk-std()-X (hertz)
o frequencyBodyAccelerometerJerk-std()-Y (hertz)
o frequencyBodyAccelerometerJerk-std()-Z (hertz)
o frequencyBodyGyroscope-mean()-X (hertz)
o frequencyBodyGyroscope-mean()-Y (hertz)
o frequencyBodyGyroscope-mean()-Z (hertz)
o frequencyBodyGyroscope-std()-X (hertz)
o frequencyBodyGyroscope-std()-Y (hertz)
o frequencyBodyGyroscope-std()-Z (hertz)
o frequencyBodyAccelerometerMagnitude-mean() (hertz)
o frequencyBodyAccelerometerMagnitude-std() (hertz)
o frequencyBodyAccelerometerJerkMagnitude-mean() (hertz)
o frequencyBodyAccelerometerJerkMagnitude-std() (hertz)
o frequencyBodyGyroscopeMagnitude-mean() (hertz)
o frequencyBodyGyroscopeMagnitude-std() (hertz)
o frequencyBodyGyroscopeJerkMagnitude-mean() (hertz)
o frequencyBodyGyroscopeJerkMagnitude-std() (hertz)

Final Dataset

str(newData)

Final Dataset summary

summary(newData)