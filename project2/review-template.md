# Code Review for _Chris Kenyon_

## Project Repo

_https://github.com/ChrisKenyon79/drinkrecipes_

## Review

#### Project Purpose

_The purpose of the project is to be able to take a single(or two) ingredient and find drink recipes utilizing the specified ingredient_

#### Project Organization

#### Features

* Random Drink 
  * Utlizing the cocktaildb random API and passes the drink data in via recipe key into the view. In the view, looped through the recipe data to populate the necessary items via EJS templates. 
* Search Function
  * Utilzing the cocktaildb search API and pass in the query. It is implemented by seperating each query into it's own array, and brought back together in combined array. The variable naming starts to get a little confusing toward the end so it get's harder to follow the trajectory.
* Favorites List
  * In each recipe view, there is an option to save it(via form method post). The favorites can be viewed in the profile and edited/deleted.

#### Areas of Success (Code, Organization)

* Attribute 1
  * The code is readable and I can understand what you are trying to achieve. 
* Attribute 2
  * The features were completed and result the expected output

#### Areas for Improvement (Code, Organization)

* Organization
  * Break out the other routes into controllers so the index.js isn't so long
* Aesthetic
  * Apply some css styling to the program 

## Additional Notes

_Place any additional notes here_
