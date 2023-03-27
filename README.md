# NoSQL Challenge

# Project Description 

## Part 1: Database and Jupyter Notebook Set Up

- Import the data and name the database/collection.
- Import libraries.
- Create an instance of Mongo Client.
- Confirm that the database is working by listing the databases in MongoDB, list the collections, and find and display one document in the establishments collection using find_one and pprint.
- Assign the establishments collection to a variable to prepare the collection for use. 


## Part 2: Update the Database

- Add a new restaurant into the database. 
- Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return the BusinessTypeID and BusinessType fileds.
- Update the new restaurant with the BusinessTypeID you found.
- Remove establishments within the Dover Local Authority and check the number of documents to make sure they were deleted.
- Use update_many to change the latitude and longitude values to decimal numbers.


## Part 3: Exploratory Analysis

- Answer the following questions: 
  - Which establishments have a hygiene score equal to 20?
  - Which establishments in London have a RatingValue greater than or equal to 4?
  - What are the top 5 establishments with a RatingValue of '5', sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
  - How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.


## Part 1: Database and Jupyter Notebook Set Up
- `mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json`
- Dependencies:
  - from pymongo import MongoClient
  - import json
  - import requests 
  - from pprint import pprint

## Part 3: Exploratory Analysis
- Dependencies:
  - from pymongo import MongoClient
  - import json
  - import requests 
  - from pprint import pprint
  - import pandas as pd 

# Output/Analyses

## Part 1: Database and Jupyter Notebook Set Up

- Imported the data and libraries.
<img width="1159" alt="Screenshot 2023-03-27 at 4 16 48 PM" src="https://user-images.githubusercontent.com/119909433/228068670-dcd6166c-3524-4c19-b1e3-c2df5bfc5403.png">

- Created an instance of MongoClient.
<img width="1151" alt="Screenshot 2023-03-27 at 4 17 24 PM" src="https://user-images.githubusercontent.com/119909433/228068790-e4256b92-8d3f-4fcf-971e-e96ca4ff87ca.png">

- Confirmed that the database was created by listing the databases, assigning the collection to a name, reviewing the collections in the database, and reviewing a document in the collection. 
<img width="1167" alt="Screenshot 2023-03-27 at 4 18 50 PM" src="https://user-images.githubusercontent.com/119909433/228069064-7551d79e-54a8-4ad6-8fe1-96bc7d31479b.png">

- Assigned the collection to a variable.
<img width="1163" alt="Screenshot 2023-03-27 at 4 19 40 PM" src="https://user-images.githubusercontent.com/119909433/228069189-26e78b66-b1b5-4bb8-b7fa-2e83b62bfdab.png">


## Part 2: Update the Database

- Added a new restaurant to the collection. 
<img width="1162" alt="Screenshot 2023-03-27 at 4 20 22 PM" src="https://user-images.githubusercontent.com/119909433/228069317-ef1c0241-1c9a-44ba-ad77-9fe8a236689d.png">

- Checked that the restaurant was added to the collection. 
<img width="1155" alt="Screenshot 2023-03-27 at 4 20 53 PM" src="https://user-images.githubusercontent.com/119909433/228069401-f789b721-62bb-48a9-a98c-f31342f2b838.png">

- Found the BusinessTypeID for "Restaurant/Cafe/Canteen" and returned the BusinessTypeID and BusinessType fields. 
<img width="1165" alt="Screenshot 2023-03-27 at 4 22 16 PM" src="https://user-images.githubusercontent.com/119909433/228069655-d8ad284a-df3a-4a18-9d68-87132bef68a1.png">

- Updated the new restaurant with the BusinessTypeID I found. 
<img width="1163" alt="Screenshot 2023-03-27 at 4 22 59 PM" src="https://user-images.githubusercontent.com/119909433/228069783-24164c07-565e-42b6-8c35-329d56faf201.png">

- !!!!!

- Changed the data type from string to decimal for latitude/longitude and check that the coordinates are numbers. 
<img width="1173" alt="Screenshot 2023-03-27 at 4 25 51 PM" src="https://user-images.githubusercontent.com/119909433/228070326-c802ff71-27e2-4eed-87a8-427544ede9fc.png">
<img width="1153" alt="Screenshot 2023-03-27 at 4 26 11 PM" src="https://user-images.githubusercontent.com/119909433/228070390-cfbe3137-e07f-49af-af76-c85f20103413.png">


## Part 3: Exploratory Analysis

- Created a query for establishments with a hygiene score equal to 20 and displayed the first document. 
<img width="1170" alt="Screenshot 2023-03-27 at 4 29 05 PM" src="https://user-images.githubusercontent.com/119909433/228070881-8a9df14a-d97f-4fd4-8aff-0ce47dd12b99.png">

- Converted the results to a DataFrame and displayed the DataFrame.
<img width="1173" alt="Screenshot 2023-03-27 at 4 29 39 PM" src="https://user-images.githubusercontent.com/119909433/228070977-f21260b5-ac30-4245-aed3-2ff82eb90e01.png">

- Created a query for establishments in London with a rating value greater than or equal to 4 and displayed the first document.

- Converted the results to a DataFrame and displayed the DataFrame.

- Created a query to find the top 5 establishments with a rating value of 5, sorted by lowest hygiene score, located nearest to the restaurant "Penang Flavours."

- Converted the results to a DataFrame and displayed the DataFrame.

- Created a query to find establishments in each Local Authority area with a hygiene score of 0.

- Converted the results to a DataFrame and displayed the DataFrame. 

# Authors 
- Brittany Wright github:brittanynicole7
