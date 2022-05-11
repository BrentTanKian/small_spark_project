# small_spark_project
This is a small Spark project where the original .py file was gotten from https://github.com/PacktPublishing/Frank-Kanes-Taming-Big-Data-with-Apache-Spark-and-Python.
The original script cleans and transforms a dataset containing 100000 movie titles, their respective ratings, genres and more, and recommends 10 other movies you should
watch, if you entered/liked a particular movie. I've went on to make some small minor improvements to the script, adding a new dataframe that contains each movie ID and its
respective average rating, and using this dataframe to filter away movies in our final selection with an average rating below 3, because we don't want to be recommending 
crappy movies do we? 

Instructions to use the script
1. After cloning down the code, look for the movie ID that you would like to receive recommendations for in the u.item file found in the ml-100k folder.
2. Go to the terminal and enter the following command: spark-submit movie-similarities-dataframe.py <Insert movie ID of choice here>
3. And the output you get will be similar to what is in the capture.png file
