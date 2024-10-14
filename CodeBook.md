# Code Book for Human Activity Recognition Using Smartphones Data

This code book describes the variables, the data, and transformations performed to create the tidy dataset `tidy_data.txt`.

## Source of Data:

The data was obtained from: [http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)

## Data Transformations:

1. **Merging:** Training and test data were merged to create a single dataset.
2. **Feature Extraction:** Only measurements on the mean and standard deviation for each measurement were extracted. These features were identified by the patterns "mean()" and "std()" in the feature names.
3. **Activity Labeling:** Activity codes (1-6) were replaced with descriptive activity names:
    * 1 WALKING
    * 2 WALKING_UPSTAIRS
    * 3 WALKING_DOWNSTAIRS
    * 4 SITTING
    * 5 STANDING
    * 6 LAYING
4. **Variable Labeling:** Descriptive variable names were used, based on the original feature names.
5. **Tidy Data Creation:** The final tidy dataset contains the average of each variable for each activity and each subject.

## Tidy Data Variables:

* **subject:** The ID of the subject who performed the activity (integer).
* **activity:** The type of activity performed (character).

* **tBodyAcc-mean()-X:** Mean of body acceleration in the X direction.
* **tBodyAcc-mean()-Y:** Mean of body acceleration in the Y direction.
* **tBodyAcc-mean()-Z:** Mean of body acceleration in the Z direction.
* **tBodyAcc-std()-X:** Standard deviation of body acceleration in the X direction.
* **tBodyAcc-std()-Y:** Standard deviation of body acceleration in the Y direction.
* **tBodyAcc-std()-Z:** Standard deviation of body acceleration in the Z direction.
* **tGravityAcc-mean()-X:** Mean of gravity acceleration in the X direction.
* **tGravityAcc-mean()-Y:** Mean of gravity acceleration in the Y direction.
* **tGravityAcc-mean()-Z:** Mean of gravity acceleration in the Z direction.
* **tGravityAcc-std()-X:** Standard deviation of gravity acceleration in the X direction.
* **tGravityAcc-std()-Y:** Standard deviation of gravity acceleration in the Y direction.
* **tGravityAcc-std()-Z:** Standard deviation of gravity acceleration in the Z direction.
  ...


[**IMPORTANT:** Continue this list with ALL variables present in the `tidy_data.txt` file and a brief description for EACH. The easiest way to get the full list is to run the `run_analysis.R` script and then use `names(tidy_data)` within R.  This will give you the precise names to use here.]