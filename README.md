# nosql-challenge
Project Summary: Food Hygiene Ratings Analysis for Eat Safe, Love Magazine

## Intro
The project aims to assist Eat Safe, Love magazine in selecting establishments to focus their future articles on by analyzing food hygiene ratings data provided by the UK Food Standards Agency. The project is divided into three parts: database and Jupyter Notebook setup, updating the database, and exploratory analysis.

## Part 1
Note: Parts 1 and 2 are located on the NoSQL setup starter ipynb
In Part 1, a NoSQL database named "uk_food" is created, and the "establishments" collection is imported from the "establishments.json" file. The required libraries, PyMongo and PPrint, are imported, and a connection to the MongoDB client is established. The successful creation of the database and collection is confirmed by listing the database and collection, and a sample document from the "establishments" collection is displayed.

## Part 2
Part 2 focuses on updating the database according to the magazine editors' requests. A new halal restaurant, Penang Flavours, is added to the database with the necessary information. The BusinessTypeID for "Restaurant/Cafe/Canteen" is found and assigned to the new restaurant. The number of documents containing the Dover Local Authority is checked, and establishments within Dover are removed from the database. Lastly, number values stored as strings are converted to numeric values using the update_many method.

## Part 3
Note: Parts 1 and 2 are located on the NoSQL analysis starter ipynb
Part 3 involves exploratory analysis of the database to answer specific questions posed by Eat Safe, Love magazine. Each question requires counting documents, displaying the first document, converting the results to a Pandas DataFrame, and displaying the first 10 rows. The questions include identifying establishments with a hygiene score of 20, establishments in London with a RatingValue greater than or equal to 4, the top 5 establishments with a RatingValue of 5 sorted by lowest hygiene score and proximity to "Penang Flavours," and the count of establishments in each Local Authority area with a hygiene score of 0, sorted from highest to lowest, with the top ten local authority areas printed.

By analyzing the food hygiene ratings data and providing answers to the magazine's questions, this project will aid Eat Safe, Love in making informed decisions about future article focuses and help their journalists and food critics select establishments that meet their standards of hygiene and quality.