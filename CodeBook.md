## HUMAN ACTIVITY RECOGNITION USING SMARTPHONES DATASET - README
Author: Stanislav Gerasymenko


---
The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz.  
  
Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag).  
  
Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals).  
  
These signals were used to estimate variables of the feature vector for each pattern ('_XYZ' is used to denote 3-axial signals in the X, Y and Z directions:

1       tBodyAcc_XYZ  
2	tGravityAcc_XYZ  
3	tBodyAccJerk_XYZ  
4	tBodyGyro_XYZ  
5	tBodyGyroJerk_XYZ  
6	tBodyAccMag  
7	tGravityAccMag  
8	tBodyAccJerkMag  
9	tBodyGyroMag  
10	tBodyGyroJerkMag  
11	fBodyAcc_XYZ  
12	fBodyAccJerk_XYZ  
13	fBodyGyro_XYZ  
14	fBodyAccMag  
15	fBodyAccJerkMag  
16	fBodyGyroMag  
17	fBodyGyroJerkMag  
  
  
  
The set of variables that were estimated from these signals are:  
  
1       mean: Mean value  
2       std: Standard deviation  
  
  
  
Below is the complete list of the resultant variables:  
  
1       fBodyAcc_mean_X  
2	fBodyAcc_mean_Y  
3	fBodyAcc_mean_Z  
4	fBodyAcc_std_X  
5	fBodyAcc_std_Y  
6	fBodyAcc_std_Z  
7	fBodyAccJerk_mean_X  
8	fBodyAccJerk_mean_Y  
9	fBodyAccJerk_mean_Z  
10	fBodyAccJerk_std_X  
11	fBodyAccJerk_std_Y  
12	fBodyAccJerk_std_Z  
13	fBodyAccJerkMag_mean  
14	fBodyAccJerkMag_std  
15	fBodyAccMag_mean  
16	fBodyAccMag_std  
17	fBodyGyro_mean_X  
18	fBodyGyro_mean_Y  
19	fBodyGyro_mean_Z  
20	fBodyGyro_std_X  
21	fBodyGyro_std_Y  
22	fBodyGyro_std_Z  
23	fBodyGyroJerkMag_mean  
24	fBodyGyroJerkMag_std  
25	fBodyGyroMag_mean  
26	fBodyGyroMag_std  
27	tBodyAcc_mean_X  
28	tBodyAcc_mean_Y  
29	tBodyAcc_mean_Z  
30	tBodyAcc_std_X  
31	tBodyAcc_std_Y  
32	tBodyAcc_std_Z  
33	tBodyAccJerk_mean_X  
34	tBodyAccJerk_mean_Y  
35	tBodyAccJerk_mean_Z  
36	tBodyAccJerk_std_X  
37	tBodyAccJerk_std_Y  
38	tBodyAccJerk_std_Z  
39	tBodyAccJerkMag_mean  
40	tBodyAccJerkMag_std  
41	tBodyAccMag_mean  
42	tBodyAccMag_std  
43	tBodyGyro_mean_X  
44	tBodyGyro_mean_Y  
45	tBodyGyro_mean_Z  
46	tBodyGyro_std_X  
47	tBodyGyro_std_Y  
48	tBodyGyro_std_Z  
49	tBodyGyroJerk_mean_X  
50	tBodyGyroJerk_mean_Y  
51	tBodyGyroJerk_mean_Z  
52	tBodyGyroJerk_std_X  
53	tBodyGyroJerk_std_Y  
54	tBodyGyroJerk_std_Z  
55	tBodyGyroJerkMag_mean  
56	tBodyGyroJerkMag_std  
57	tBodyGyroMag_mean  
58	tBodyGyroMag_std  
59	tGravityAcc_mean_X  
60	tGravityAcc_mean_Y  
61	tGravityAcc_mean_Z  
62	tGravityAcc_std_X  
63	tGravityAcc_std_Y  
64	tGravityAcc_std_Z  
65	tGravityAccMag_mean  
66	tGravityAccMag_std  
  
  
  
During both training and testing phases of the experiment, the above variables were estimated for 30 subjects (persons):  
  
1-30  
  
  
  
while each subject performed the the following activities:  
  
1       WALKING  
2	WALKING_UPSTAIRS  
3	WALKING_DOWNSTAIRS  
4	SITTING  
5	STANDING  
6	LAYING  
  
  
  
After that, the variables were grouped by subject and activity, by applying the mean function to the 66 variables mentioned above. The following variables were created as a result:  
  
1       meanOf_fBodyAcc_mean_X  
2	meanOf_fBodyAcc_mean_Y  
3	meanOf_fBodyAcc_mean_Z  
4	meanOf_fBodyAcc_std_X  
5	meanOf_fBodyAcc_std_Y  
6	meanOf_fBodyAcc_std_Z  
7	meanOf_fBodyAccJerk_mean_X  
8	meanOf_fBodyAccJerk_mean_Y  
9	meanOf_fBodyAccJerk_mean_Z  
10	meanOf_fBodyAccJerk_std_X  
11	meanOf_fBodyAccJerk_std_Y  
12	meanOf_fBodyAccJerk_std_Z  
13	meanOf_fBodyAccJerkMag_mean  
14	meanOf_fBodyAccJerkMag_std  
15	meanOf_fBodyAccMag_mean  
16	meanOf_fBodyAccMag_std  
17	meanOf_fBodyGyro_mean_X  
18	meanOf_fBodyGyro_mean_Y  
19	meanOf_fBodyGyro_mean_Z  
20	meanOf_fBodyGyro_std_X  
21	meanOf_fBodyGyro_std_Y  
22	meanOf_fBodyGyro_std_Z  
23	meanOf_fBodyGyroJerkMag_mean  
24	meanOf_fBodyGyroJerkMag_std  
25	meanOf_fBodyGyroMag_mean  
26	meanOf_fBodyGyroMag_std  
27	meanOf_tBodyAcc_mean_X  
28	meanOf_tBodyAcc_mean_Y  
29	meanOf_tBodyAcc_mean_Z  
30	meanOf_tBodyAcc_std_X  
31	meanOf_tBodyAcc_std_Y  
32	meanOf_tBodyAcc_std_Z  
33	meanOf_tBodyAccJerk_mean_X  
34	meanOf_tBodyAccJerk_mean_Y  
35	meanOf_tBodyAccJerk_mean_Z  
36	meanOf_tBodyAccJerk_std_X  
37	meanOf_tBodyAccJerk_std_Y  
38	meanOf_tBodyAccJerk_std_Z  
39	meanOf_tBodyAccJerkMag_mean  
40	meanOf_tBodyAccJerkMag_std  
41	meanOf_tBodyAccMag_mean  
42	meanOf_tBodyAccMag_std  
43	meanOf_tBodyGyro_mean_X  
44	meanOf_tBodyGyro_mean_Y  
45	meanOf_tBodyGyro_mean_Z  
46	meanOf_tBodyGyro_std_X  
47	meanOf_tBodyGyro_std_Y  
48	meanOf_tBodyGyro_std_Z  
49	meanOf_tBodyGyroJerk_mean_X  
50	meanOf_tBodyGyroJerk_mean_Y  
51	meanOf_tBodyGyroJerk_mean_Z  
52	meanOf_tBodyGyroJerk_std_X  
53	meanOf_tBodyGyroJerk_std_Y  
54	meanOf_tBodyGyroJerk_std_Z  
55	meanOf_tBodyGyroJerkMag_mean  
56	meanOf_tBodyGyroJerkMag_std  
57	meanOf_tBodyGyroMag_mean  
58	meanOf_tBodyGyroMag_std  
59	meanOf_tGravityAcc_mean_X  
60	meanOf_tGravityAcc_mean_Y  
61	meanOf_tGravityAcc_mean_Z  
62	meanOf_tGravityAcc_std_X  
63	meanOf_tGravityAcc_std_Y  
64	meanOf_tGravityAcc_std_Z  
65	meanOf_tGravityAccMag_mean  
66	meanOf_tGravityAccMag_std  
  
  
  