# NoSQL_Challenge
UK Food Establishments Analysis
This project involves setting up a NoSQL database using MongoDB, importing and modifying data, and performing exploratory analysis on UK food establishments.

Part 1: Database and Jupyter Notebook Set Up
In this part, we import the data provided in the establishments.json file using MongoDB's mongoimport command. The database is named uk_food and the collection is named establishments.

We then use a Jupyter notebook to interact with our database. The necessary libraries, PyMongo and Pretty Print (pprint), are imported. An instance of the Mongo Client is created and we confirm that the database and data were loaded properly.

Part 2: Database Modifications
In this part, we make several modifications to the establishments collection based on specific requirements.

A new restaurant is added to the database. The BusinessTypeID for "Restaurant/Cafe/Canteen" is found and used to update the new restaurant's data.

Establishments within the Dover Local Authority are removed from the database.

Some data types are also converted. The latitude and longitude values are converted to decimal numbers, and the RatingValue is converted to integer numbers.

Part 3: Exploratory Analysis
In this part, we answer specific questions to help find the locations the magazine wishes to visit and avoid.

We find establishments with a hygiene score equal to 20, establishments in London with a RatingValue greater than or equal to 4, and the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours".

We also find how many establishments in each Local Authority area have a hygiene score of 0 and sort the results from highest to lowest.

The results are displayed using count_documents to display the number of documents contained in the result, pprint to display the first document in the results, and Pandas DataFrames to display the first 10 rows of the results.
