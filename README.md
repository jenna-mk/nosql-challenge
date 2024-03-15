# Module 12 Challenge: An Analysis of UK Food Establishments With NoSQL
The purpose of this challenge is to perform an in-depth analysis of various food and beverage establishments across the United Kingdom, according to evaluations by the UK Food Standards Agency. This analysis is completed by use of MongoDB, a NoSQL database management program. 

## Part 1: Database and Jupyter Notebook Set Up
In the first part of this challenge, I set up the database environment for analysis. In the first step, I imported the data from the establishment.json file (Starter_Code/Resources) into a new database called 'uk_food' and a new collection 'establishments'. Next, I imported the required libraries (PyMongo and Pretty Print), created an instance of Mongo Client, and confirmed the creation of my collection and database. The code for Part 1 is found in Starter_Code/NoSQL_setup_starter.ipynb.

## Part 2: Update the Database
In the second part of this challenge, I updated the database to ensure that it included all business information desired in the correct datatype. I added a newly opened restaurant, updated its BusinessTypeID to match the id for "Restaurant/Cafe/Canteen", removed all establishments in Dover, and converted the latitude/longitude to decimal numbers and the RatingValue to integer for all establishments. The code for Part 2 is found in Starter_Code/NoSQL_setup_starter.ipynb.

## Part 3: Exploratory Analysis
The final part of this challenge involves analyzing certain aspects of the data in order to inform people on the best (and worst) restaurants to visit in a given area. The questions are as follows:

1.) Which establishments have a hygiene score equal to 20?

I found 41 total establishments with a hygiene score equal to 20 (for context, hygiene scores are reverse rated, so the higher the score, the worse the rating).

2.) Which establishments in London have a rating value greater than or equal to 4?

I found 33 total establishments in London with a rating value greater than or equal to 4.

3.) What are the top 5 establishments with a rating value of 5, sorted by lowest hygiene score, closest to the newly opened Penang Flavours restaurant?

The top 5 establishments near Penang Flavours, in order of best hygiene score, are Volunteer (pub/bar/nightclub), Atlantic Fish Bar (takeaway/sandwich shop), Lumbini Grocery Ltd T/A Al-Iman (retailers - other), Iceland (retailers - supermarkets/hypermarkets), and Howe and Co Fish and Chips - Van 17 (mobile caterer).

4.) How many establishments in each local authority area have a hygiene score of 0?

There are 55 local authority areas, each with various numbers of establishments that meet the requirement for hygiene score of 0. The full results for this question (as well as all other code for Part 3) is found in Starter_Code/NoSQL_analysis_starter.ipynb. 

## References
UK Food Standards AgencyLinks to an external site. (2022). UK food hygiene rating data API. https://ratings.food.gov.uk/open-data/en-GBLinks to an external site.. Contains public sector information licensed under the Open Government Licence v3.0Links to an external site.
Accessed Sept 9, 2022 and Sept 12, 2022 with the establishment settings as follows: longitude=51.5072, latitude=-0.1276, maxdistancelimit=4567, pagesize=10000, sortoptionkey=distance, pagenumber=(1,2,3,4,5,6,7,8).
