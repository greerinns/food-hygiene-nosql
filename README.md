# Food Hygiene Ratings Analysis for Eat Safe, Love Magazine

## Project Summary

This project serves as an analytical endeavor aimed at supporting Eat Safe, Love magazine in the selection of establishments to feature in their future articles. The analysis is based on food hygiene ratings data provided by the UK Food Standards Agency. The project unfolds in three distinct parts, encompassing database setup, database updates, and exploratory analysis.

## Part 1: NoSQL Database Setup

*Note: Parts 1 and 2 are located within the NoSQL setup starter notebook.*

In Part 1, we initiate the process by establishing a NoSQL database named "uk_food." This database is populated with the "establishments" collection, imported from the "establishments.json" file. The essential libraries, namely PyMongo and PPrint, are imported to facilitate the task. We establish a connection to the MongoDB client and verify the successful creation of the database and collection. A sample document from the "establishments" collection is presented for reference.

## Part 2: Database Update

Part 2 of the project revolves around accommodating the specific requests made by the magazine's editors. Key tasks in this phase include the addition of a new halal restaurant, "Penang Flavours," to the database with all relevant information. We diligently determine the BusinessTypeID for "Restaurant/Cafe/Canteen" and associate it with the new restaurant entry. Furthermore, we inspect the count of documents containing the Dover Local Authority and subsequently remove establishments within the Dover region from the database. Finally, we address the issue of numeric values stored as strings by employing the update_many method.

## Part 3: Exploratory Analysis

*Note: Parts 1 and 2 are located within the NoSQL analysis starter notebook.*

The heart of the project lies in Part 3, where we embark on an exploratory analysis of the database. Our objective is to provide precise answers to specific queries posed by Eat Safe, Love magazine. Each inquiry necessitates a series of steps, including document counting, display of the initial document, conversion of results into a Pandas DataFrame, and presentation of the first 10 rows. Our analysis tackles questions such as identifying establishments with a hygiene score of 20, pinpointing establishments in London with a RatingValue greater than or equal to 4, listing the top 5 establishments with a RatingValue of 5, sorted by the lowest hygiene score and proximity to "Penang Flavours," and revealing the count of establishments in each Local Authority area with a hygiene score of 0. The results are thoughtfully organized, with the top ten local authority areas listed in descending order.

By meticulously analyzing food hygiene ratings data and delivering precise responses to the magazine's inquiries, this project aims to empower Eat Safe, Love in making well-informed decisions regarding the focus of their future articles. This data-driven approach will assist their journalists and food critics in selecting establishments that align with their stringent standards of hygiene and quality.
