# nosql-challenge
Challenge 12 of UoB Data Analytics bootcamp - NoSQL databases

# About the repository:
This repository contains:
- Jupyter Notebook ['NoSQL_setup_starter.ipynb'](https://github.com/catisf/nosql-challenge/blob/main/NoSQL_setup_starter.ipynb)
- Jupyter Notebook ['NoSQL_analysis_starter.ipynb'](https://github.com/catisf/nosql-challenge/blob/main/NoSQL_analysis_starter.ipynb)
- [Resources folder](https://github.com/catisf/nosql-challenge/tree/main/Resources), which contains 'establishments.json' data file.

In order to run the repository, the following dependencies need to be installed/imported:
- pymongo
- pprint
- pandas

# About the challenge:
## Deliverables:
- Deliverable 1: A Jupyter notebook containing code that imports the data and sets up and updates the uk_food database (['NoSQL_setup_starter.ipynb'](https://github.com/catisf/nosql-challenge/blob/main/NoSQL_setup_starter.ipynb));
- Deliverable 2: A Jupyter notebook containing code that performs the exploratory analysis queries in the database (['NoSQL_setup_starter.ipynb'](https://github.com/catisf/nosql-challenge/blob/main/NoSQL_setup_starter.ipynb)).
- 
## Part 1: Setup
- Using ['NoSQL_setup_starter.ipynb'](https://github.com/catisf/nosql-challenge/blob/main/NoSQL_setup_starter.ipynb):
  - Import the data in the 'establishments.json' file. Name the database uk_food and the collection establishments. The notebook includes details on how to import the data and assign the correct name to the database and the collection;
  - Import the necessary libraries: PyMongo and Pretty Print (pprint);
  - Create an instance of the Mongo Client;
  - Confirm that the database was created and loaded the data properly.

## Part 2: Update the Database 
- Using ['NoSQL_setup_starter.ipynb'](https://github.com/catisf/nosql-challenge/blob/main/NoSQL_setup_starter.ipynb):
  - Add a new restaurant to the Database;
  - Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields;
  - Update the new restaurant with the BusinessTypeID found;
  - Check how many documents contain the Dover Local Authority. Then, remove any establishments within the Dover Local Authority from the database, and check the number of     documents to ensure they were deleted;
  - Update datatypes (using update_many).

## Part 3: Exploratory Analysis
- Using ['NoSQL_analysis_starter.ipynb'](https://github.com/catisf/nosql-challenge/blob/main/NoSQL_analysis_starter.ipynb) answer the following questions:
  - Which establishments have a hygiene score equal to 20?
  - Which establishments in London have a RatingValue greater than or equal to 4?
  - What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
  - How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
