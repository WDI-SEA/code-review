# Code Review for Leo Burke

## Project Repo

https://github.com/boetw/project2

## Review

#### Project Purpose

This project allows users to do a search for lego sets based on a keyword, save them to a profile, and manage their saved favorites.

#### Project Organization

#### Features

* Api Search
  * Site allows you to query the api and it returns a list of lego sets based on that keyword
* Favorite sets
  * Site allows logged in users to save lego sets to their profile

#### Areas of Success (Code, Organization)

* EJS layouts
  * Successful use of EJS partials to make elements of the site
* API implementation
  * Neat use of an obscure API

#### Areas for Improvement (Code, Organization)

* API key not obscured by .env file
  * To make an api call the api key is in the JS file in plain text and not as an ENV variable.
* Lots of commented out code
  * Certain features seem to have been turned off at the last minute
* No readme file
  * Don't have clear install instructions or a point to see where the app is installed.

## Additional Notes

Tried getting it working, node didn't want to cooperate. Looks like the API is back up, so maybe try re-implementing the functionality. 

Generally a good start to something I would find useful, but you should really get that API key in the env file, and get the project working and deployed.
