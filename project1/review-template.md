# Code Review for Thomas Evans

## Project Repo

https://github.com/evans760/1-10-in-Sapanish-Game

## Review

#### Project Purpose

The purpose of the project is to teach a child or children how to count to 10 in Spanish.

#### Project Organization

#### Features

* Clickable Numbers Corresponding to Word Choice Above
  * After an image is shown and a number is clicked, a jQuery listener is attached to that div's contents and a function is run (parseInt()) to compare the div's contents to the corresponding key value in the words array. If they match up, the answer is correct and that object's index is removed from the array using splice().
* Hideable Instructions
  * Using SweetAlert, the instructions are placed above the game area and are able to be hidden once understood.
* Restart Game Button That Doesn't Refresh Page
  * The button resets the game counter to zero and, if I'm understanding correctly, resets the words array to its original state.

#### Areas of Success (Code, Organization)

* Most Variables Are Named Well
  * Using variables with names such as 'gamelogic' and 'reset()' made it far easier to understand what each function does.
* Bootstrap and SweetAlert Are Well-Implemented
  * The use of Bootstrap lays out the page well, while SweetAlert is a nice way to get quick feedback.

#### Areas for Improvement (Code, Organization)

* Never Know How Many Numbers Are Left
  * It might be nice to know how many numbers are left to be clicked, but it could also be part of the game design, so as not to indirectly give away any answers.
* Clickable Numbers Could Be Better Formatted
  * Making the clickable numbers into buttons, or simply surrounding each number div with a border, may help the interface even though it wouldn't change the functionality of the game.
* Have Instructions Able to Reappear
  * It may be a nice feature to have the instructions reappear if the player gets confused.

## Additional Notes

Great start!  I think this is a great foundation to build upon a children's learning game.
