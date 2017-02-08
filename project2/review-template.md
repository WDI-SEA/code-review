# Code Review for Dan Rasmussen

## Project Repo

https://github.com/imdanras/project2

## Review

#### Project Purpose

The Burger of the Month webapp's purpose is to take in a location search and return results about all of the nearest restaurants that server Burgers!

#### Project Organization

#### Features

* API Call to Yelp for search results
  * Uses a GET route to Yelps search functionality, passing in the term "burger" each time. Also is setting the search location based on either input from the client, or the clients current location.
* Ability to save restaurants to a favorites list
  * Uses  a POST route to create an entry in a database based on the users id and the restaurants id. This also has the ability to be removed from the database
* Ability to update the users profile 
  * Uses a PUT route to call update on the database entry based on the current users id

#### Areas of Success (Code, Organization)

*Code seems well organized, easy to read, and almost entirely semantically labeled

#### Areas for Improvement (Code, Organization)

* Maybe work on removing console logs that no longer are needed as well as removing unneccessary comment blocks

## Additional Notes

Let me start by saying, good job Dan, I think this project turned out well. 

Functionality changes I would make would be, changing the redirect on the delete functionality, currently it takes you away from the favorites list when you delete an entry, maybe doing a redirect to the same list page would work? The favorites page could also use a little bit of "labeling", the list doesn't tell me what it is exactly, and maybe the update button could be set up in a different spot. I would do away with the stringified JSON that appears at the top also.
