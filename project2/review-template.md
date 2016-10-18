# Code Review for _Insert Name Here_

## Project Repo

https://github.com/dropTheNon/Project-2

## Review

#### Project Purpose

To help the organization of both Hackathon creators and of it's members. By centralizing all users to one website, a currated list can be created and used as a roster for multiple events.

#### Project Organization

#### Features

* Local Login
  * This project utilizes SQL for keeping track of users across sessions.
  * By utilizing custom middleware, users can only access certain pages while logged in.
* Relational Database
  * By organizing the database into many tables and linking them together by their appropriate foreign keys, space is saved, data is organized and optimized for the server. The level of organization is exceedingly.
* Multiple Titles
  * Thanks to the structure of the database, a user can have more than one attribute. It all matters based on context. All people are users. A user has a many to many relation with titles, based on the open project. Because a user is a organizer on one project, does not automatically make them a organizer in another. 

#### Areas of Success (Code, Organization)

* Database Execution
  * Impecible! Every table has only the bare minimum that pertains to each table. Each table is then compared against others to form more meaningful data per context that it is called!
* Middleware
  * The use of custom middleware kept organization and code to a minimum. This way, if a user is not an Organizer, or is not a Registered, or even Logged In, they will not be granted access for the route. Minimized quite a bit of code and left the routes clean and clear.

#### Areas for Improvement (Code, Organization)

* Instruction on Cloning Repo
  * Getting started has no instructions past NPM install. A user has to go through the steps of removing the non-working authentication and seting up the database on their own.
* Styling
  * Function > Form. With that said, mimicing another site is a great way to have that official/professional feel in as minimal time as possible :)

## Additional Notes

This Hackathon organizer is a swell idea. Tighten up the loose ends (auth, CSS) and throw it up on the internet!
