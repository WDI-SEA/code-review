# Code Review for Joe M.

## Project Repo

*https://github.com/jmarzu/fridge
*https://joe-fridge.herokuapp.com

## Review

#### Project Purpose

**Fridge management application*
*A user can search for recipes using the ingredients they have in their fridge.
*A user can build up a collection of recipes and save them to their profile to view later.
*A user can create a shopping list and enter in and expiration date. This data is saved for later use.

#### Project Organization

#### Features

* User search uses an API and returns results based on ingredients passed in
  * Searching your fridge involves making a GET request to the recipepuppy API. 
  * The form/search bar appends a .query string to the URL. Ther returned data is
  * displayed on an EJS page.
* User can save search results to a database table for later viewing (must be logged in)
  * Once the user is on the search results EJS page, they can save recipes for later through
  * the use of a hidden form. When the user clicks the "Save Recipe" button they are actually
  * submitting form data to a POST route which checks if the user is logged in and writes the body
  * of the form and some other user data to a database table.
* User can add items to his/her fridge with the expected expiration date (must be logged in)
  * User enters in a string and a date, the .body of the form inputs is pushed to a database table

#### Areas of Success (Code, Organization)

* Organization
  * The organization is great
* Clarity of Purpose
  * This app does exactly what it set out to do and is easily iterated upon

#### Areas for Improvement (Code, Organization)

* Styles
  * I'd change the background or font colors around a bit to make things easier to see

## Additional Notes

*I liked hearing Joe's presentation about growing this idea from a "seed." He has plans to extend this project and I like that he plans to pursue this idea and strengthen the app as he gains more skills as a programmer.
