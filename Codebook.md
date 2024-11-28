# Code Book for Tidy Dataset

## Overview
This code book describes the variables and transformations applied to the Samsung wearable computing dataset to create a tidy data set.

## Variables
- `subject`: The ID of the participant (1–30).
- `activity`: The activity being performed (e.g., WALKING, SITTING).
- Measurement variables (e.g., `tBodyAcc-mean()-X`, `tBodyAcc-std()-Y`):
  - Mean and standard deviation of accelerometer and gyroscope signals for each axis.

## Transformations
1. Merged the training and test datasets.
2. Extracted measurements on mean and standard deviation for each observation.
3. Replaced activity codes with descriptive names.
4. Labeled dataset with descriptive variable names.
5. Created a tidy dataset with the average of each variable for each activity and subject.
