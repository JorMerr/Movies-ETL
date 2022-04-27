# Movies-ETL

## Overview of Project

The purpose of this project is to gather movie data from different sources then clean, organize, and merge data to be used in a company sponsored hackathon. 
The task of taking in new data, performing transformations, and loading to SQL tables has been automated using a function for ease of use in order to allow the company to update their information on a daily basis.

## Summary

Extracting the raw data from our initial dataset allowed the large initial files to be read and transformed more easily. One difficulty in storing the project data in GitHub was that the original files were of a size too large to be held remotely. The solution to this challenge was to update the .gitignore file to ignore those larger files. 

Once the initial function was created, the code was then used to create the appropriate DataFrames for each dataset, finally merging them into our DataFrame, movies_df. The movies_df DataFrame was then loaded to our pgAdmin SQL Database to store as flat files. The below image confirms that the required number of rows of data were correctly loaded into SQL as the 'movies' table.

![movies_query](https://github.com/JorMerr/Movies-ETL/blob/main/Resources/movies_query.PNG)

The following image shows the much larger ratings_file storing the transformed data from the original ratings.csv file has been loaded correctly. 

![ratings_query](https://github.com/JorMerr/Movies-ETL/blob/main/Resources/ratings_query.PNG)

The original ratings.csv file was one of the larger file sizes of our original dataset at approximately 692MB, much larger than the file size limit for GitHub remote storage. 

