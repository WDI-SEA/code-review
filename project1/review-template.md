# Code Review for _Insert Name Here_

## Project Repo

https://github.com/ivarmlee11/squareFall

## Review

#### Project Purpose

The main objective of the game is to stay alive as long as possible while you are falling. Hitting any object will bring your velocity to zero. You know what they say: "It's not the fall that kills you, it's the sudden stop"

#### Project Organization

#### Features

* Scoring
  * Scoring is implemented purely on a timed basis. When you die, the loop that time is based off of closes. Therefore score can no longer be incremented.
* Falling
  * The coordinates of the player actually don't change, rather it is the obsticles that move upwards. Each obsticle is an object that containes a position function which updates every game tick.
* Collision
  * Collision is tricky. Each obsticle object contains the [single axis] coordinates of each side. Every game tick, compare the coordinates of the player with the [single axis] coordinates of each obsticle. If any of them meet, then this means a collision has occured.
* Scoring
  * All scores are maintained in an online database known as FireBase. This service makes it as easy as possible to maintain simple data in an array. Firebase has it's own way to manage the array, however it is as simple as .child(playerName).set() to set a score. 

#### Areas of Success (Code, Organization)

* Collision Detection
  * How collisions are detected are handled inside each object and with minimal chained if statements to compare 'areas of squares' sharing the same coordinate space.
* Scoring
  * The use of Firebase as a online database for scores is a huge plus because everyone can now battle each other and maintain dominance with proof.

#### Areas for Improvement (Code, Organization)

* Firebase
  * All Firebase actions could be done inside one Firebase object. This would organize and group the code for better management, maintainability and less variable declaration (variables declared on the spot for self referencing).
* Game Object
  * The Canvas related functions could also be put into an object for better organization. As well as having everything outside of 'on document ready' (still using 'on document ready', but have everything called from outside it).

Everything is really well done, simple organization would increase readability tenfold! Amazing job on the comments, without them I would have been lost.

## Additional Notes

I made changes to the game in the form of a pull request. This way we can go over them in person. I figure you will want to do it yourself, but this way you have something to look at and we have things to discuss in person.
