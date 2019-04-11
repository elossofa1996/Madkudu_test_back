# Madkudu_test_back
This project is my work for madkudu test

The back end was developed using express(NodeJS)
Library used:
    "http": "0.0.0", -> To send request for a third actor
    "http-errors": "~1.6.2", -> To send Http Error response
    "http-status-codes": "^1.3.2", -> To add status code in the header reponse
    "joi": "^14.3.1", ->Used to valid body request and valid inputs and give a schema for objects
    "mongodb": "^3.2.2", -> Using mongodb database
    "mongoose": "^5.4.20", -> ODM
I use a complex architecture for my project:
In the Api folder: Contains controller and routes of each entity
	In the constants: field.js -> An array of each field in the antelope document in the databse
			  horns.js -> An array of each type of antelope horns
In the config folder:
	express.js -> Contains configuration of the express
	index.js -> contains the env variables, ports and URL(URI)
In the lib folder:
	Contains Joi library with external modules for Date and ObjectId(like in the mongo database)
In the models folder:
	Contains entitys and the communication with the database and querys