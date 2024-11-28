# Getting and Cleaning Data - Course Project

This repository contains the R code and related files for the *Getting and Cleaning Data* course project.

## Files

1. **`run_analysis.R`**  
   - This script processes the Samsung dataset to create a tidy data set.
   - It assumes that the dataset is extracted to the working directory in a folder named `UCI HAR Dataset`.

2. **`CodeBook.md`**  
   - This file describes the variables, data, and transformations performed to prepare the tidy data set.

3. **`README.md`**  
   - This file explains the contents of the repository and how to run the analysis.

## How to Run the Analysis

1. **Download the Dataset**  
   - Download the dataset from [here](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip).
   - Extract the contents into your working directory. For example:  
     ```
     C:\Users\yourname\Documents\R\UCI HAR Dataset
     ```

2. **Run the Script**  
   - Open R or RStudio and set the working directory to the folder containing `run_analysis.R`.
   - Run the script using:  
     ```R
     source("run_analysis.R")
     ```

3. **Output**  
   - The script generates a file named `data_set_with_the_averages.txt` in the working directory, which contains the tidy data set.

---

### Example `CodeBook.md`
```markdown
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
