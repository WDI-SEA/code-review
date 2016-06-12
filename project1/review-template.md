# Code Review for Jamie Karlovich

## Project Repo

https://github.com/jkarlovich

## Review

#### Project Purpose

The purpose of this project was to build a 2048 clone using HTML, CSS, javascript, and Jquery.

#### Project Organization

#### Features

* Feature 1
  *The first feature that i think is super cool is the functions that get called on the key press to add up your numbers and move numbers over. The way that Jamie did this was by looping through her row length or column length and using the JQuery trim() and text() methods in her "if" check she looks to see if there is any numbers stacked up in the direction of the arrow key that you hit. In doing this she can then decide if the numbers should add stack or stay put. 
* Feature 2
  *The second feature is how Jamie was able to get a pair of matching numbers to add in one move, but if there were a set of 4 matching numbers in a row she was able to prevent those numbers from totaling, because in 2048 only two numbers in a row or column of the same type can add in one move. The way she implemented this was do an if check to see what direction was hit on the arrow keys. Then use a for loop to check her board array for stacked matching numbers. If any matching sets were found the farthest one in the coresponding direction would have its value multiplied by 2, and the other number would have its value set to a blank string. At the same time the square that had its number multiplied would be added a class called stop. She then used this class in a if check to stop if from continuing to add if there were to be a matching square next to it after the initial add. Then after exiting this key down function the stop classes would be removed so the squares can be added again. 
* Feature 3
  *Jamies game board is 4 nested arrays of 4 Jquery id calls. So in every if check she makes she uses this board with x,y cordinates to see how her game is changing.

#### Areas of Success (Code, Organization)

* Attribute 1
  *The js file is very clean and orginized. She wrote functions for specific perposes and uses all of them. Everything is named well.
* Attribute 2
  *Her page looks great too. I'm terrible at css, so I can appreciate a simple clean build.

#### Areas for Improvement (Code, Organization)

* Attribute 1
  * I would say that there can be some major refactoring done on her js file to her "if" checks. There are 4 key press funcitons and corresponding if checks. So maybe there could be just one key press function and one check for that function. But thats a little above my head right now.
* Attribute 2
  * Her check to see if the board is full could probably be refactored as well. Instead of checking the text length to see if any square has a value and calling it on every square. Maybe you could use the array reduce function and see if a certain value gets returned when every square is full. 

## Additional Notes

Im super impressed by this game! Amazing work.
