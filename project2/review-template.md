# Code Review for SmithTM90

## Project Repo

[https://github.com/SmithTM90/Twitter-Lorem]

## Review

#### Project Purpose

_List the purpose and components of the project here_

The purpose of the project is to be able to search Twitter using their API and generate random text with the returned API call results. Users can choose the number of lorem sentences to be generated. A user can also save particular results to favorites.


#### Project Organization

#### Features

* Searches Twitter's API using a query
  * Calls Twitter's API using a POST method
* Search results can be of different sentence lengths
  * A drop-down menu stores a value and then uses that chosen value to return that number of popular tweets.
* User can save favorite twitter lorem results
  * If favorited, the search result will be saved to the database and identified by a user's ID

#### Areas of Success (Code, Organization)

* Successfully makes the API call using the search query
  * It's great because it does exactly what it says it does and it does it well
* Can save to favorites
  * Very useful since each search could potentially bring back vastly different results
* Code organization
  * Code is very well organized and easy to read

#### Areas for Improvement (Code, Organization)

* NSFW?
  * I'm not sure how to implement it, but something like a 'kid-friendly' checkbox could be helpful
* Non-letters
  * Not sure how to implement this either, but it would be nice if there was a way to filter out non-letter and/or numbers

## Additional Notes

Great job. The app does exactly what it's supposed to and does it cleanly.
