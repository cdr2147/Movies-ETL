# Movies-ETL
## Overview
Amazing Prime is preparing for a hackathon. Amazing Prime needs to gather data from both Wikipedia and Kaggle, combine them, and save them into a SQL database so that the hackathon participants have a nice, clean dataset to use. We followed the ETL process to prepare this data: extract the Wikipedia and Kaggle data from their respective files, transform the datasets by cleaning them up and joining them together, and load the cleaned dataset into a SQL database.

## Purpose
After the ETL process, Amazing Prime wants to keep the data updated on a daily basis for the hackathon. We are asked to create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. We refactor the code from this module to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—and performs the ETL process by adding the data to a PostgreSQL database.

## Results
Refactoring the code and calling the extract_transform_load() function cleaned all the data and created tables in the SQL database. Our query to the SQL database
shows that all rows of data were properly imported. Using this function is helpful because it can be easily updated.
![Code snapshot](https://user-images.githubusercontent.com/99205688/163841632-3336e3ae-8900-480e-8a8f-b2b0f9eadadb.PNG)

![movies_query](https://user-images.githubusercontent.com/99205688/163840890-92c41545-8de8-48f4-a1de-c6ee24217e5a.PNG)

![ratings_query](https://user-images.githubusercontent.com/99205688/163840895-24726333-09a4-43ac-8970-3ceed0bc9144.PNG)
