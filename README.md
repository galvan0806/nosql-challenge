# nosql-challenge

This challenge is divided into 3 parts where Part 1 and Part 2 are done in NoSQL_setup_starter.ipynb and Part 3 is done in NoSQL_analysis_starter.ipynb.

In this challenge, I have been contracted by the food magazine editors, Eat Safe, Love, to evaluate some of the ratings data iand assist their journalists and food critics to decide what articles to focus on in the future.
 
## Part 1: Database and Jupyter Notebook Set Up
Use NoSQL_setup_starter.ipynb for this section of the challenge. 

1.Import the data provided in the establishments.json file from your Terminal. Name the database uk_food and the collection establishments. Copy the text you used to import your data from your Terminal to a markdown cell in your notebook.

2.Within your notebook, import the libraries you need: PyMongo and Pretty Print (pprint).

3.Create an instance of the Mongo Client.

4.Confirm that you created the database and loaded the data properly:

5.Assign the establishments collection to a variable to prepare the collection for use.


## Part 2: Update the Database
Use NoSQL_setup_starter.ipynb for this section of the challenge. 

1.An exciting new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked you to include it in your analysis. Add the following information to the database:

    {
    "BusinessName":"Penang Flavours",
    "BusinessType":"Restaurant/Cafe/Canteen",
    "BusinessTypeID":"",
    "AddressLine1":"Penang Flavours",
    "AddressLine2":"146A Plumstead Rd",
    "AddressLine3":"London",
    "AddressLine4":"",
    "PostCode":"SE18 7DY",
    "Phone":"",
    "LocalAuthorityCode":"511",
    "LocalAuthorityName":"Greenwich",
    "LocalAuthorityWebSite":"http://www.royalgreenwich.gov.uk",
    "LocalAuthorityEmailAddress":"health@royalgreenwich.gov.uk",
    "scores":{
        "Hygiene":"",
        "Structural":"",
        "ConfidenceInManagement":""
    },
    "SchemeType":"FHRS",
    "geocode":{
        "longitude":"0.08384000",
        "latitude":"51.49014200"
    },
    "RightToReply":"",
    "Distance":4623.9723280747176,
    "NewRatingPending":True
    }

2.Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.

3.Update the new restaurant with the BusinessTypeID you found.

4.The magazine is not interested in any establishments in Dover, so check how many documents contain the Dover Local Authority. Then, remove any establishments within the Dover Local Authority from the database, and check the number of documents to ensure they were deleted.

5.Some of the number values are stored as strings, when they should be stored as numbers.

## Part 3: Exploratory Analysis
Use NoSQL_analysis_starter.ipynb for this section of the challenge. 

1.Which establishments have a hygiene score equal to 20?

2.Which establishments in London have a RatingValue greater than or equal to 4?

3.What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?

4.How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.



## Sources:

Boot Camp Module 12