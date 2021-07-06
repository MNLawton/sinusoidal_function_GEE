# sinusoidal_function_GEE

This workflow uses GEE
1.	Copy the “sinosoidal function” into GEE.  
2.	Define your study area as “study_area” and select a single point called “single_pixel”
3.	Edit “start_time” and “end_time” to your dates
4.	Edit “year_of_first_break” to one year after the start date (such that if your “start_time” is 1989-01-01, “year_of_first_break” would equal 1990)
5.	Edit the final number in “years” to equal the total number of years the study will use to create the sinosoidal function
6.	In the FOR loop, set statement 2 (“i<_”) to the total number of years in the study minus 1.  
7.	Run the script
8.	These images are exported to google drive
In a new script, open “change_detection”
9.	Import from google drive the change layer and name it “change_layer”
10.	Import from google drive the no-change layer and name it “no_change_layer”
11.	Edit statement 1 to the minimum threshold value you wish to test multiplied by 100 (such if you wish to use a threshold of 0.98, use 98)
12.	Edit statement 2 to the maximum threshold value you wish to test, as before
13.	Edit “change_start” to the year you would like change detection to commence (e.g. 2003)
14.	Edit “change_end” to the final year you wish to detect change for (e.g. 2011 detects change up to 31st of December 2011)
15.	Run the script
16.	These layers are exported to google drive
In a new script open “classification”
17.	Upload and import your ground truth data (this is automatically named “table”)
18.	Import your image you wish to classify (this is automatically named “image”)
19.	Define your study area (this is automatically named “geometry”)
20.	Run the script
21.	Image is exported to google drive
