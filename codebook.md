For each record it is provided:
======================================

- A 561-feature vector with time and frequency domain variables. 
- Its activity label. 
- An identifier of the subject who carried out the experiment.

The dataset includes the following files:
=========================================

**- 'features_info.txt': Shows information about the variables used on the feature vector. These are as follows:**

mean(): Mean value
std(): Standard deviation
mad(): Median absolute deviation 
max(): Largest value in array
min(): Smallest value in array
sma(): Signal magnitude area
energy(): Energy measure. Sum of the squares divided by the number of values. 
iqr(): Interquartile range 
entropy(): Signal entropy
arCoeff(): Autorregresion coefficients with Burg order equal to 4
correlation(): correlation coefficient between two signals
maxInds(): index of the frequency component with largest magnitude
meanFreq(): Weighted average of the frequency components to obtain a mean frequency
skewness(): skewness of the frequency domain signal 
kurtosis(): kurtosis of the frequency domain signal 
bandsEnergy(): Energy of a frequency interval within the 64 bins of the FFT of each window.
angle(): Angle between to vectors.

- 'features.txt': List of all features.

**- 'activity_labels.txt': Links the class labels with their activity name. These are as follows:**

WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING

**- 'train/X_train.txt': Training set**

Contains the 561-feature vector with time and frequency domain variables for each observation for the training set

**- 'train/y_train.txt': Training labels.**

Identifies the participant (1 - 30) 

**- 'test/X_test.txt': Test set.**

Contains the 561-feature vector with time and frequency domain variables for each observation for the test set

**- 'test/y_test.txt': Test labels.**

Identifies the participant (1 - 30)
