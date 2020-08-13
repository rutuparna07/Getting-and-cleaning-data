# Code book:

The data set that this code book pertains to is located in the `tidy_data.txt` file of this repository.

See the `README.md` file of this repository for background information on this data set.

The structure of the data set is described in the [Data](#data) section, its variables are listed in the [Variables](#variables) section, and the transformations that were carried out to obtain the data set based on the source data are presented in the [Transformations](#transformations) section.

The tidydataset is the result of appling the 5 steps from the week 4 project of 
the Getting and Cleaning coruse in coursera.

The data was extracted from the data set placed in this Url
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 
Inside of it you can find the files used in this project: **features.txt, activity_labels.txt, subject_test.txt, X_test.txt, y_test.txt, subject_train.txt, X_train.txt, y_train.txt**.

the tidydata data set, wich is the result of these project is, is compounded by 
the means and standar deviation, by subject and actvity, of the existing varibles founded in the **features.txt** file applied to the (*"test and train"*) files wich were bind by row and made one single table.


*[1] "subject"                                                    
 [2] "activity"                                                   
 [3] "Time Body Accelerometer Mean ()X"                           
 [4] "Time Body Accelerometer Mean ()Y"                           
 [5] "Time Body Accelerometer Mean ()Z"                           
 [6] "Time Gravity Accelerometer Mean ()X"                        
 [7] "Time Gravity Accelerometer Mean ()Y"                        
 [8] "Time Gravity Accelerometer Mean ()Z"                        
 [9] "Time Body Accelerometer JerkMean ()X"                       
[10] "Time Body Accelerometer JerkMean ()Y"                       
[11] "Time Body Accelerometer JerkMean ()Z"                       
[12] "Time Body Gyroscope Mean ()X"                               
[13] "Time Body Gyroscope Mean ()Y"                               
[14] "Time Body Gyroscope Mean ()Z"                               
[15] "Time Body Gyroscope JerkMean ()X"                           
[16] "Time Body Gyroscope JerkMean ()Y"                           
[17] "Time Body Gyroscope JerkMean ()Z"                           
[18] "Time Body Accelerometer Magnitude Mean ()"                  
[19] "Time Gravity Accelerometer Magnitude Mean ()"               
[20] "Time Body Accelerometer JerkMagnitude Mean ()"              
[21] "Time Body Gyroscope Magnitude Mean ()"                      
[22] "Time Body Gyroscope JerkMagnitude Mean ()"                  
[23] "Frequency Body Accelerometer Mean ()X"                      
[24] "Frequency Body Accelerometer Mean ()Y"                      
[25] "Frequency Body Accelerometer Mean ()Z"                      
[26] "Frequency Body Accelerometer Mean Freq()X"                  
[27] "Frequency Body Accelerometer Mean Freq()Y"                  
[28] "Frequency Body Accelerometer Mean Freq()Z"                  
[29] "Frequency Body Accelerometer JerkMean ()X"                  
[30] "Frequency Body Accelerometer JerkMean ()Y"                  
[31] "Frequency Body Accelerometer JerkMean ()Z"                  
[32] "Frequency Body Accelerometer JerkMean Freq()X"              
[33] "Frequency Body Accelerometer JerkMean Freq()Y"              
[34] "Frequency Body Accelerometer JerkMean Freq()Z"              
[35] "Frequency Body Gyroscope Mean ()X"                          
[36] "Frequency Body Gyroscope Mean ()Y"                          
[37] "Frequency Body Gyroscope Mean ()Z"                          
[38] "Frequency Body Gyroscope Mean Freq()X"                      
[39] "Frequency Body Gyroscope Mean Freq()Y"                      
[40] "Frequency Body Gyroscope Mean Freq()Z"                      
[41] "Frequency Body Accelerometer Magnitude Mean ()"             
[42] "Frequency Body Accelerometer Magnitude Mean Freq()"         
[43] "Frequency Body Body Accelerometer JerkMagnitude Mean ()"    
[44] "Frequency Body Body Accelerometer JerkMagnitude Mean Freq()"
[45] "Frequency Body Body Gyroscope Magnitude Mean ()"            
[46] "Frequency Body Body Gyroscope Magnitude Mean Freq()"        
[47] "Frequency Body Body Gyroscope JerkMagnitude Mean ()"        
[48] "Frequency Body Body Gyroscope JerkMagnitude Mean Freq()"    
[49] "Angle (TimeBody  Accelerometer Mean,gravity)"               
[50] "Angle (TimeBody  Accelerometer JerkMean),gravityMean)"      
[51] "Angle (TimeBody  Gyroscope Mean,gravityMean)"               
[52] "Angle (TimeBody  Gyroscope JerkMean,gravityMean)"           
[53] "Angle (X,gravityMean)"                                      
[54] "Angle (Y,gravityMean)"                                      
[55] "Angle (Z,gravityMean)"                                      
[56] "Time Body Accelerometer STD ()X"                            
[57] "Time Body Accelerometer STD ()Y"                            
[58] "Time Body Accelerometer STD ()Z"                            
[59] "Time Gravity Accelerometer STD ()X"                         
[60] "Time Gravity Accelerometer STD ()Y"                         
[61] "Time Gravity Accelerometer STD ()Z"                         
[62] "Time Body Accelerometer JerkSTD ()X"                        
[63] "Time Body Accelerometer JerkSTD ()Y"                        
[64] "Time Body Accelerometer JerkSTD ()Z"                        
[65] "Time Body Gyroscope STD ()X"                                
[66] "Time Body Gyroscope STD ()Y"                                
[67] "Time Body Gyroscope STD ()Z"                                
[68] "Time Body Gyroscope JerkSTD ()X"                            
[69] "Time Body Gyroscope JerkSTD ()Y"                            
[70] "Time Body Gyroscope JerkSTD ()Z"                            
[71] "Time Body Accelerometer Magnitude STD ()"                   
[72] "Time Gravity Accelerometer Magnitude STD ()"                
[73] "Time Body Accelerometer JerkMagnitude STD ()"               
[74] "Time Body Gyroscope Magnitude STD ()"                       
[75] "Time Body Gyroscope JerkMagnitude STD ()"                   
[76] "Frequency Body Accelerometer STD ()X"                       
[77] "Frequency Body Accelerometer STD ()Y"                       
[78] "Frequency Body Accelerometer STD ()Z"                       
[79] "Frequency Body Accelerometer JerkSTD ()X"                   
[80] "Frequency Body Accelerometer JerkSTD ()Y"                   
[81] "Frequency Body Accelerometer JerkSTD ()Z"                   
[82] "Frequency Body Gyroscope STD ()X"                           
[83] "Frequency Body Gyroscope STD ()Y"                           
[84] "Frequency Body Gyroscope STD ()Z"                           
[85] "Frequency Body Accelerometer Magnitude STD ()"              
[86] "Frequency Body Body Accelerometer JerkMagnitude STD ()"    
[87] "Frequency Body Body Gyroscope Magnitude STD ()"             
[88] "Frequency Body Body Gyroscope JerkMagnitude STD ()"* 




## Variables <a name="variables"></a>

Each row contains, for a given subject and activity, 79 averaged signal measurements.

### Identifiers <a name="identifiers"></a>

- `subject`

	Subject identifier, integer, ranges from 1 to 30.

- `activity`

	Activity identifier, string with 6 possible values: 
	- `WALKING`: subject was walking
	- `WALKING_UPSTAIRS`: subject was walking upstairs
	- `WALKING_DOWNSTAIRS`: subject was walking downstairs
	- `SITTING`: subject was sitting
	- `STANDING`: subject was standing
	- `LAYING`: subject was laying

### Average of measurements <a name="average-measurements"></a>

All measurements are floating-point values, normalised and bounded within [-1,1].

Prior to normalisation, acceleration measurements (variables containing `Accelerometer`) were made in *g*'s (9.81 m.s⁻²) and gyroscope measurements (variables containing `Gyroscope`) were made in radians per second (rad.s⁻¹).

Magnitudes of three-dimensional signals (variables containing `Magnitude`) were calculated using the Euclidean norm.

The measurements are classified in two domains:

- Time-domain signals (variables prefixed by `timeDomain`), resulting from the capture of accelerometer and gyroscope raw signals.

- Frequency-domain signals (variables prefixed by `frequencyDomain`), resulting from the application of a Fast Fourier Transform (FFT) to some of the time-domain signals.


The zip file containing the source data is located at [https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip).

The following transformations were applied to the source data:

1. The training and test sets were merged to create one data set.
1. The measurements on the mean and standard deviation (i.e. signals containing the strings `mean` and `std`) were extracted for each measurement, and the others were discarded.
1. The activity identifiers (originally coded as integers between 1 and 6) were replaced with descriptive activity names (see [Identifiers](#identifiers) section).
1. The variable names were replaced with descriptive variable names (e.g. `tBodyAcc-mean()-X` was expanded to `timeDomainBodyAccelerometerMeanX`), using the following set of rules:
	- Special characters (i.e. `(`, `)`, and `-`) were removed
	- The initial `f` and `t` were expanded to `frequencyDomain` and `timeDomain` respectively.
	- `Acc`, `Gyro`, `Mag`, `Freq`, `mean`, and `std` were replaced with `Accelerometer`, `Gyroscope`, `Magnitude`, `Frequency`, `Mean`, and `StandardDeviation` respectively.
	- Replaced (supposedly incorrect as per source's `features_info.txt` file) `BodyBody` with `Body`.
1. From the data set in step 4, the final data set was created with the average of each variable for each activity and each subject.

The collection of the source data and the transformations listed above were implemented by the `run_analysis.R` R script (see `README.md` file for usage instructions).


## Data <a name="data"></a>

The `tidy_data.txt` data file is a text file, containing space-separated values.

The first row contains the names of the variables, which are listed and described in the [Variables](#variables) section, and the following rows contain the values of these variables. 
