# Code Review for Chris Madison

## Project Repo

https://github.com/CMadison/Connect4

## Review

#### Project Purpose

This is a 2-player game that has players alternate turns dropping a colored disc into a grid system, with the goal being to get 4 of your colored pieces in a row.

#### Project Organization

#### Features

* Feature 1
  * Clicking the top row of the grid lets you drop a piece into that column.
* Feature 2
  * Play automatically switches between colors
* Feature 3
  * The game alerts a win when one player has 4 pieces in a row.

#### Areas of Success (Code, Organization)

* Organization of Code
  * Most functions were well-commented, which helped in understanding the purpose of said function
* CSS
  * Clean and simple game, which I love.

#### Areas for Improvement (Code, Organization)

* Win Condition Bug
  * I know you're still working on diagonal win condition, but there is a bug in horizontal win condition - horizontal connect 4's that touch the right wall aren't counted, and the game continues.
* Commenting
  * Most functions were well commented, with the exception of the code in app.js, lns 43-74, which was harder to parse without the clear comments you left elsewhere (you spoiled me, Chris!).

## Additional Notes

Good stuff, Maynard.  Get those win conditions fixed, and you're all set with a clean-looking portfolio piece.  :-)
