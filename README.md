# GetAndCleanDataProject

The plyr library is used in this solution.

I first merge the training data and test sets, thus creating one data set.

This codes gets the wearable data from the Internet, then computes the average of the means and standard deviations of the accelerometer and gyroscope data of all who participated in the research.

## Requirements

This script makes use of `plyr`

## Usage from R Studio

source("run_analysis.R")

## How the script works... 

1. Downloads the data and saves it in the data subdirectory of the working directory.
2. Data is extracted to the current working directory. 
3. Merges the training and test "features" data into a single extract.
4. Merges training and test label data, then converts the numeric labels to a familiar label.
5. Merges the training and test subject label data together.
6. Combines the features, label and subject data sets into one unified data set.
6. Calculates the average of each mean and standard deviation of each metric of each participant and activity.

### Processing Methodology

The original data set is download and extracted in the working directory and the following files are used:
- ./UCI HAR Dataset/features.txt
- ./UCI HAR Dataset/activity_labels.txt
- ./UCI HAR Dataset/test/X_test.txt
- ./UCI HAR Dataset/train/X_train.txt
- ./UCI HAR Dataset/test/y_test.txt
- ./UCI HAR Dataset/train/y_train.txt
- ./UCI HAR Dataset/test/subject_test.txt
- ./UCI HAR Dataset/train/subject_train.txt

The ./UCI HAR Dataset/features.txt is used indexing and naming

These are the activity labels/values.
1. Walking
2. Walking Upstairs
3. Walking Downstairs
4. Sitting
5. Standing
6. Laying


