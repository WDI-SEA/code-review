# Code Review for _Insert Name Here_

## Project Repo

https://github.com/kamsci/SwitchIT

## Review

#### Project Purpose

To interperet and review the code for the game SwitchIt.

#### Project Organization

#### Features

There are few main files: html, css, javascript, jQuery, sweet alerts

* Feature 1
  * The html page holds the containers that that the board will be made in. The board is not made in the html file, but in the javascript file. There are scrips that are held in this file. The link to css, and jQuery. There is also a script for Sweet Alerts which is very successfull. The page is also responsive. 

* Feature 2
  * The CSS page is organized very well. The only tags that are used are div tags and class names. Which is very proper use of the css tags. 
    The monsters all have their own color and there is a lot of hard coded in code. However, all the monsters are defined well and it's easy to read code. 

* Feature 3
  * The javascript file holds 2 arrays that hold the data for the monsters and also data for the game board. The game board is actually created by a function call setUpBoard(). A random monster is chosed by a function, createRandomMonster(), and the piece can be swtiched around by the next function createSwitchPiece.

  1. function createRandomMonster()
    generates a randome monster picture from the array of objects

2. function createSwitchPiece()
    calls the createRandomMonster function and 
    creates the piece to switch with a game board piece

3. function setUpBoard()
    This function iterates over an empty array and sets up divs of columns and rows to create the board. This is an awesome technique because the game board can vary for each level giving even more complexity to the game. 

4. function switchPiece()
    This switches the piece on the board with the swtich piece

5. The next few functions collect the points and check if there are any rows or columns of pieces with winning combinations. 

6. As the player gathers points they can level up in the game and play harder levels. 

7. The final function actually runs the game. This sounds like a great way to organize the code. The game can fully load with all the parameters before it actually runs for the user to start the game.  

#### Areas of Success (Code, Organization)

* Attribute 1
  * The code was very easy to read. It was well documented and the names of the variables and functions made it easy to understand what it was going to do. 

* Attribute 2
  * The sweet alerts were really sweet. That might be an easy observation, but it was a little touch that went a long way. 

#### Areas for Improvement (Code, Organization)

* Attribute 1
  * It's too bad we didn't learn about conductors and prototypes becuase it could have saved a lot of code to create the level and monster object arrays. 

* Attribute 2
  * This is speculation, but, it make make sense to have the compliation of the code be more compartmental then all at once. Having the game completely load and then run might take a long time if it is a huge game. This is speculation on my part. 

## Additional Notes

This is a really awesome game. It was fun to play and the code looked great. Nice Job.
