## Codebook for tidy.txt

### Introduction
This is a code book for tidy.txt.  This code book describes the variables in tidy.txt.  As explained in README.md, tidy.txt was produced using the raw Samsung data available at https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

### Variables

*"Subject": the identifier of the subject performing an activity.  There are 30 subjects, each assigned a number between 1 and 30.

*"Activity": the activity being performed.  There are 6 activities: LAYING, SITTING, STANDING, WALKING, WALKING DOWNSTAIRS, WALKING UPSTAIRS

*There are 66 variables that give the average (for a given subject and activity) of a particular measurement on the mean or standard deviation of the Samsung data.  The variable names in tidy.txt are modified (more descriptive and all lower case) versions of the variable names in the features\_info.txt (available at the url above).  Note that the measurements are normalized and bounded within [-1, 1] (so we don't need to be concerned with units for these variables).
(All measurements used to produce these averages were obtained as described in features\_info.txt.)  More precisely:

1. Names beginning with "time" concern time domain signals captured at a constant rate of 50 Hz.  

2. Names beginning with "frequency.domain.signal" concern frequency domain signals (obtained by applying a Fast Fourier Transform to time domain signals.)

3. Names ending with "x" (respectively, "y", "z") indicate measurements in the "x" (respectively, "y", "z") direction.

4. Names with "mean" (respectively "standard.deviation") concern the mean (respectively, standard deviation) of a measurement.

5. The other components of the variable names are as in features_info.txt (but converted to lower case).  In particular:
  a) "bodyacc" and "gravityacc" denote the body and gravity acceleration signals, resp.
  b) "bodyaccjerk" and "bodygyrojerk" denote the jerk signals from the body linear acceleration and angular velocity, resp.
  c) "bodyaccmag", "gravityaccmag", "bodyaccjerkmag", and "bodygyrojerkmag" denote the magnitude of the corresponding above 3-dimensional signals, calculated using the Euclidean norm

In summary, the resulting 68 variables (explained above) in tidy.txt are:

 [1] "Subject"                                                   
 [2] "Activity"                                                  
 [3] "time.bodyacc.mean.x"                                       
 [4] "time.bodyacc.mean.y"                                       
 [5] "time.bodyacc.mean.z"                                       
 [6] "time.bodyacc.standard.deviation.x"                         
 [7] "time.bodyacc.standard.deviation.y"                         
 [8] "time.bodyacc.standard.deviation.z"                         
 [9] "time.gravityacc.mean.x"                                    
[10] "time.gravityacc.mean.y"                                    
[11] "time.gravityacc.mean.z"                                    
[12] "time.gravityacc.standard.deviation.x"                      
[13] "time.gravityacc.standard.deviation.y"                      
[14] "time.gravityacc.standard.deviation.z"                      
[15] "time.bodyaccjerk.mean.x"                                   
[16] "time.bodyaccjerk.mean.y"                                   
[17] "time.bodyaccjerk.mean.z"                                   
[18] "time.bodyaccjerk.standard.deviation.x"                     
[19] "time.bodyaccjerk.standard.deviation.y"                     
[20] "time.bodyaccjerk.standard.deviation.z"                     
[21] "time.bodygyro.mean.x"                                      
[22] "time.bodygyro.mean.y"                                      
[23] "time.bodygyro.mean.z"                                      
[24] "time.bodygyro.standard.deviation.x"                        
[25] "time.bodygyro.standard.deviation.y"                        
[26] "time.bodygyro.standard.deviation.z"                        
[27] "time.bodygyrojerk.mean.x"                                  
[28] "time.bodygyrojerk.mean.y"                                  
[29] "time.bodygyrojerk.mean.z"                                  
[30] "time.bodygyrojerk.standard.deviation.x"                    
[31] "time.bodygyrojerk.standard.deviation.y"                    
[32] "time.bodygyrojerk.standard.deviation.z"                    
[33] "time.bodyaccmag.mean"                                      
[34] "time.bodyaccmag.standard.deviation"                        
[35] "time.gravityaccmag.mean"                                   
[36] "time.gravityaccmag.standard.deviation"                     
[37] "time.bodyaccjerkmag.mean"                                  
[38] "time.bodyaccjerkmag.standard.deviation"                    
[39] "time.bodygyromag.mean"                                     
[40] "time.bodygyromag.standard.deviation"                       
[41] "time.bodygyrojerkmag.mean"                                 
[42] "time.bodygyrojerkmag.standard.deviation"                   
[43] "frequency.domain.signal.bodyacc.mean.x"                    
[44] "frequency.domain.signal.bodyacc.mean.y"                    
[45] "frequency.domain.signal.bodyacc.mean.z"                    
[46] "frequency.domain.signal.bodyacc.standard.deviation.x"      
[47] "frequency.domain.signal.bodyacc.standard.deviation.y"      
[48] "frequency.domain.signal.bodyacc.standard.deviation.z"      
[49] "frequency.domain.signal.bodyaccjerk.mean.x"                
[50] "frequency.domain.signal.bodyaccjerk.mean.y"                
[51] "frequency.domain.signal.bodyaccjerk.mean.z"                
[52] "frequency.domain.signal.bodyaccjerk.standard.deviation.x"  
[53] "frequency.domain.signal.bodyaccjerk.standard.deviation.y"  
[54] "frequency.domain.signal.bodyaccjerk.standard.deviation.z"  
[55] "frequency.domain.signal.bodygyro.mean.x"                   
[56] "frequency.domain.signal.bodygyro.mean.y"                   
[57] "frequency.domain.signal.bodygyro.mean.z"                   
[58] "frequency.domain.signal.bodygyro.standard.deviation.x"     
[59] "frequency.domain.signal.bodygyro.standard.deviation.y"     
[60] "frequency.domain.signal.bodygyro.standard.deviation.z"     
[61] "frequency.domain.signal.bodyaccmag.mean"                   
[62] "frequency.domain.signal.bodyaccmag.standard.deviation"     
[63] "frequency.domain.signal.bodyaccjerkmag.mean"               
[64] "frequency.domain.signal.bodyaccjerkmag.standard.deviation" 
[65] "frequency.domain.signal.bodygyromag.mean"                  
[66] "frequency.domain.signal.bodygyromag.standard.deviation"    
[67] "frequency.domain.signal.bodygyrojerkmag.mean"              
[68] "frequency.domain.signal.bodygyrojerkmag.standard.deviation"