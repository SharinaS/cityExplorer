# City Explorer

## Code301 Lab09**Author**: Sharina Stubbs
**Version**: 1.3.0 (increment the patch/fix version number if you make more commits past your first submission)

## Overview
This is backend for a frontend application designed to allow users to input a location and display weather, local events, movies, restaurant reviews and hiking trails for that local area. This backend uses APIs and database data supplied to the frontend in a readable format to render to the frontend.

## Getting Started
### If you build from scratch, you will have to install the following packages: 
1. npm init -y
2. npm install -S express dotenv
3. npm install -S cors
4. npm install -S superagent (for working with APIs)

### If you copy the code down to your machine from my repo on GitHub, after cloning, simply:
1. Do a touch .env to create a file, then within that .env file add PORT and API keys:
* PORT=port_number
* In sum: Add environment variables to your server named: EVENTBRITE_API_KEY, WEATHER_API_KEY, GEOCODE_API_KEY, MOVIE_API_KEY, YELP_API_KEY... and use them appropriately in your code.
* Add environment variable named: DATABASE_URL, to hold appropriate postgress url
2. type npm install (to install all packages needed... about 86 packages).
3. Refresh the database by dropping all tables and creating them, if they do no already exist: Execute from the command line: psql -d city_explorer -f schema.sql 
* city_explorer is the database name, and schema.sql, is the file name for the database with in the repo.

### Front End app exists here:
https://codefellows.github.io/code-301-guide/curriculum/city-explorer-app/front-end/


### To start server:
Type into terminal: <nodemon>, then, to restart at any time, enter `rs`

### To access PostGresSQL via terminal:
* Type in: psql
* To see databases that exist: \l
* To connect to database city_explorer: \c city_explorer

## Architecture
This application was designed with
* JavaScript
* Express
* SuperAgent 
* PostGreSQL
* Node.JS

## Change Log

08-20-2019 9:15am - Put together file structure.

08-20-2019 10:00am - Created object literal to pull data from geo.json

08-20-2019 10:15am - Made object literal into a constructor function and created a new instance of the location data which is appearing and the route is responding in the deployed static client.

08-20-2019 10:35am - Deployed to Heroku.

08-20-2019 1:50pm - Weather data time is now converted from milliseconds into a date.

08-21-2019 9:40am - File structure in place for new driver's computer

08-21-2019 10:20am - Completed code review of yesterday's code

08-21-2019 10:28am - Deployed to Heroku

08-21-2019 11:28am - locations functionality completed using API

08-21-2019 11:50am - Weather functionality completed using API

08-21-2019 4pm - Events functionality in place using API

08-22-2019 9:20am - Database Created

08-22-2019 9:45am - Google map data stored in SQL database table.

08-22-2019 10:50am - Dark Sky data stored in SQL database table.

08-22-2019 11:45am - Eventbrite data stored in SQL database table.


## Credits and Collaborations on this version of cityExplorer
* Sharina Stubbs
* Susanna Lakey
* Peter Carmichael
* Jon Veach

# Features
## Number and name of feature: Tuesday Lab

Estimate of time needed to complete: 4 hours

Start time: 9am

Finish time: 2pm, minus 1 hour, plus another 45 min

Actual time needed to complete: 4 hours 45 min

## Number and name of feature: Wednesday Feature - Adding API functionality

Estimate of time needed to complete: 3 hours

Start time: 9am

Finish time: 2pm, minus 1 hour, plus another 45 min

Actual time needed to complete: 4 hours 45 min
