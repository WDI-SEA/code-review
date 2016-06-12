# Code Review for Joe Marzu

## Project Repo

https://github.com/jmarzu/Project-1-Chutes-and-Ladders

## Review

#### Project Purpose

Purpose: Turn-based games with the goal to be the first player to reach the end of the gameboard. 

Components: 
* Use of JQuery
* Boostrap was listed as a script, but does not appear to be used
* HTML gamboard with 50 squares
* Chutes as obstacles to send you away from your goal
* Ladders as assistance to send you closer to your goal
* Random number generator to give you the spaces you can move each turn

#### Project Organization

#### Features

* Implementation of Gameboard Design and Movement
  * HTML
    * Created with 50 div elements in html, each has a class of odd or even
    * Chutes and ladders pictures are added as img src in select div elements
    * p tags with IDs number 1-50 are added to each div element as well as a placeholder for the players to render as they move along the board
  * JS
    * Board array with properties:
      * "id" - numeric - used to comapre with currentSpacesMovedPlayer (sum of moves count) and determine where the player needs to be
      * "position" - string - reference to the HTML divs, used to place player in the correct postition corresponding to the div p id
      * "action" - numeric - used to add additional moves forward or backward
    * As the player moves, their images and a new p elements are appended to the corresponding html "position"
* Implementation of Turns and Dice
  * Implied button order of operations: Start Game > Spin > Move Player, however, any button can be pushed at any time
  * Spin - Random generates a number between 1 - 10 for player move, automatically alternates between players after every click using modulus to 
  * Move Player - Takes spin number position and adds any action that position has, then places player on board depending on which player is identified by spin button. If an action is taken, the player is notified with a message at the top of the board. 
  * 
* Implementation of chooseWinner
  * After every turn, this function compares currentSpacesMovedPlayer1 & 2 with a local variable, 50. If the player has moved beyond 50, they win!

#### Areas of Success (Code, Organization)

* Actions - Code/Org
  * Actions were successfully stores in the game array to reference what extra actions should be taken if the player lands in that space
* currentSpacesMovedPlayer - Org
  * A running move count for each player was useful for mapping the player location to the board without having to re-locate every turn
* Game Feel - Org
  * Super fun execution with Player images and videos, made it unique from regular chutes and ladders and fun to play

#### Areas for Improvement (Code, Organization)

* Prevention of inappropriate button clicks - Code/Org
  * Something that prevents the user from clicking the spin button, move, button, or any other button before the game is started, and again before they have actually moved. 
  Currently, a player can click spin many times and the spins are stored to count toward the move. Maybe if they had been in functions that were called sequentially they could have a flow of order... or posibly use remove listeners when buttons should not be pushed..?
* Use of .append
  * I was running into some of these issues too, but it appears that a new p tag is added to the exisitng p everytime the player is moved. It seems this also prevents 2 players form being in the same square.
* Separation between player move and board action - Org
  * Currently the player dice move is added to the board action so they happen simultaneously, it would be nice to add a deplay so the user knows what action is happening separate from their roll.


## Additional Notes

Great original spin on an existing idea. I like where you were going with this code too, there are just a few features that need to be polished and might have been caught with some additional testing. TDD might help this process now! I think the place to focus on code-wise is sequencing to make sure the players can't do whatever they want with button pressing order. The game was pretty good until i started pressing buttons in any order i wanted, then the messages to the user did not match up with what the code was doing. 
