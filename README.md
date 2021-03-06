# Movies-ETL
Module 8: ETL - Extract, Transform, Load

## Project Overview
The purpose of this project is to help Britta to prepare dataset for the hackathon and create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. To do this, we will follow the ETL process: extract the Wikipedia and Kaggle data from their respective files, transform the datasets by cleaning them up and joining them together, and load the cleaned dataset into a SQL database.

## Resources
Data Source: ratings.csv, wikipedia-movies.json, movies_metadata.csv

Software: ProsgreSQL, PGAdmin, Python 3.9.0, Anaconda Navigator 2.1.1, Jupyter Notebook 6.4.6

## Results
### Deliverable 1: Write an ETL Function to Read Three Data Files
- ETL function 
<img src="Images/D1img1.png" width="50%" height="50%">

- The *wiki_movies_df* DataFrame
<img src="Images/D1img2.png" width="50%" height="50%">

- The *kaggle_metadata* DataFrame
<img src="Images/D1img3.png" width="50%" height="50%">

- The *ratings* DataFrame
<img src="Images/D1img4.png" width="25%" height="25%">

### Deliverable 2: Extract and Transform the Wikipedia Data
- *wiki_movies_df* DataFrame
<img src="Images/D2img1.png" width="50%" height="50%">

- A try-except block is used to catch errors while extracting the IMDb IDs with a regular expression and dropping duplicate IDs
<img src="Images/D2img3.png" width="50%" height="50%">

- add the columns from *wiki_movies_df* DataFrame to a list
<img src="Images/D2img2.png" width="25%" height="25%">

### Deliverable 3: Extract and Transform the Kaggle data
- *movies_with_ratings_df* DataFrame 
<img src="Images/D3img1.png" width="50%" height="50%">

- *movies_df* DataFrame
<img src="Images/D3img2.png" width="50%" height="50%">

### Deliverable 4: Create the Movie Database
- The data from the movies_df DataFrame replaces the current data in the movies table in the SQL database, as determined by the *movies_query.png*
<img src="Images/movies_query.png" width="50%" height="50%">

- The data from the MovieLens rating CSV file is added to the ratings table in the SQL database, as determined by the *ratings_query.png*.
<img src="Images/ratings_query.png" width="50%" height="50%">

- The elapsed time to add the data to the database is displayed in the *ETL_create_database.ipynb* file
<img src="Images/D4img1.png" width="50%" height="50%">
