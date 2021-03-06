Samsung-Project
===============

**EXPERIMENT DESCRIPTION**

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING UPSTAIRS, WALKING DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.

**EXPLANATION OF HOW THE CODE WORKS**

The file called, Tidy Data Set, contains the code that will collect, clean and summarize the data from the accelerometers from the Samsung Galaxy S smartphone.

The 'Tidy Data Set' code will do the following:

**Download and Read the Data**

Created a file in the working directory called 'data'. Then download and unzip the UCI HAR Dataset in this file. Then read the training data set that identifies the subjects who took part in the experiment and then labelled this vector "Participant". The participant vector is stored in the variable 'subjectTrain'

Next, read the training data set that contains all the reading from the 561 various measurements and store this in the variable called 'subjectTrainX'. Then read the 561 measurement labels and set these as the column headers for the 'subjectTrainX' data frame.

Read the data that idicates which activity the participant was taking (i.e. WALKING, WALKING UPSTAIRS, WALKING_DOWNSTAIRS,SITTING,STANDING, LAYING). This was stored in the variable 'subjectTrainY'

**Merging the Data**

The next step is to merge the two vectors that contain the participant number and activity undertaken, along with the data frame of the 561 differing measurements.

This was repeated exactly the same way for the data sets set up for the 'Test' data, which were merged to form the data frame, 'testdata'.

Both the training data set(trainingdata) and the test data set(testdata) were merged to form the combined data and stored in the variable called 'combined.

**Label the Data**

The activity labels were then replaced with the corresponding activity label('1'='Walking', '2'='Walking Upstair', '3'='Walking_Downstairs', '4'='Sitting', '5'='Standing', '6'='Laying')

**Combine, Group and Summarise the Data**

The combined data frame(combined) was then converted to class tbl_df. From this it will do the following:
  1. convert the 'combined' data set from wide format to long format so that 561 measurement variables become on variable labelled, 'features'.
  2. group the data set by the 561 different measurement features, then the type of activity, and then by the participant.
  3. summarize the results to obtain the average(mean) of each variable(features) for each activity and each participant

**Filter and Select the Data**

Finally, filter the summarized data to contain only variables that contain the mean measurement readings. These are then stored in the variable, 'tidydata'.
