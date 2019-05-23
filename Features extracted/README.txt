*************************************************************************************
				FEATURES EXTRACTED FOLDER
*************************************************************************************
_____________________________________________________________________________________
CONTENT OF THE FOLDER
_____________________________________________________________________________________
This folder contains the csv files of each audiofile used. The name of each file
represents de audio file. The following table shows more detail of what each file 
contents.

The filename is composed for 4 digits: 00XY.wav, the X represents the candidate which 
has an specific level: Expert (E), Mid-level (M), Low-level (L). The Y represents the 
exercise played.

+---------------+-------+	+---------------+-------------------------------+
|  filename	| level	|	|    Exercise	| Name of the exercise		|
+---------------+-------+	+---------------+-------------------------------+
| 000Y.wav	|   M	|	|     00X1.wav	|  9. Pizzicato			|
+---------------+-------+	+---------------+-------------------------------+
| 001Y.wav	|   M  	|	|     00X2.wav	| 14. Kreutzer 4		|
+---------------+-------+	+---------------+-------------------------------+
| 002Y.wav	|   M	|	|     00X3.wav	| 18. Schradieck 1,1		|
+---------------+-------+	+---------------+-------------------------------+
| 003Y.wav	|   E	|	|     00X8.wav	| 30. G Major Scale Detache	|
+---------------+-------+	+---------------+-------------------------------+
| 004Y.wav	|   E	|	|     00X9.wav	| 35. D Major Scale Long Legato	|
+---------------+-------+	+---------------+-------------------------------+
| 005Y.wav	|   E	|	|     00X0.wav	| 36. Chromatic Scale		|
+---------------+-------+	+---------------+-------------------------------+
| 006Y.wav	|   L	|
+---------------+-------+	* Note that the last exercise increase the tens
| 007Y.wav	|   L	|	
+---------------+-------+	So, for example, the file 0053.wav is the exercise 
				nº 18 played by an expert. 
_____________________________________________________________________________________
CONTENT OF EACH FILE
_____________________________________________________________________________________
Each file contains 20 rows of the following features:  pitch, centroid, flatness, 
rolloff, zero-crossing and the first 15 MFCC - there're in order.

In case where the FFT is used, I set a windows of 1024 and a hop-size of 512. All
the features are reduced by 10 using a median filter in order to reduce the data
and also de noise.
