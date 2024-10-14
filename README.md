# Human Activity Recognition Using Smartphones Data Analysis

This repository contains the R script (`run_analysis.R`) used to clean and process the "Human Activity Recognition Using Smartphones" dataset. The script performs the following steps:

1. **Downloads and extracts the dataset:** Downloads the zip file from the specified URL and extracts it to a "data" directory.

2. **Merges the training and the test data:** Reads the training and test data files (X, y, and subject) and combines them into single datasets.

3. **Extracts mean and standard deviation measurements:** Filters the data to keep only the columns representing mean and standard deviation measurements.

4. **Uses descriptive activity names:** Replaces the numeric activity codes with descriptive activity labels (e.g., "WALKING", "STANDING").

5. **Labels the dataset with descriptive variable names:** Applies descriptive names to the variables in the dataset.

6. **Creates a tidy dataset:** Calculates the average of each variable for each activity and each subject, creating a new tidy dataset. This tidy dataset is written to a file named "tidy_data.txt".

## How to run the script:

1. Make sure you have R and the required package (dplyr) installed.
2. Download this repository.
3. Open R and change the directory to the location of the `run_analysis.R` script.
4. Run the script using the following command: `source("run_analysis.R")`

This will create the `tidy_data.txt` file in the same directory.

## Contents of tidy_data.txt:

The `tidy_data.txt` file contains the resulting tidy dataset produced by the script.  Each row represents the average of each variable for each activity and each subject.

