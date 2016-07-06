# Code Review for Derek Robertson

## Project Repo

[Project](https://github.com/d-robertson/Project-Brain-Storm/blob/master/src/index.html)
[Game](http://d-robertson.github.io/Project-Brain-Storm/)

## Review

#### Project Purpose

This is a typing game in which words fall from the top of the screen down to the bottom.  The goal is to type in as many words as possible correctly before they hit the bottom of the screen.  You start with a timer giving you 60 seconds to type as many words as possible.  Every word you destroy, you get 5 points added to your score.  Every time you get 3 words correct, 3 seconds is added to the timer.  You get penalized one point everytime you use the backspace.

#### Project Organization

#### Features

* Loading Icon
  * Create div with a class in html and set class to display:hidden in css
  * After at the end of the boot state, the load state is called
  * Once the load state is called, the div gets set to display:block so the player can see it
  * The spinner is animated with a transition element of rotate from 0 degrees to 360 degrees and keeps repeating until the ajax call is complete, in which the loading icon gets set to hidden again.
* Use of animation on both Menu and Play state
  * sets the div's scroll of tilePosition.y to += 1 or 2
* Adds adds points to the score counter
  * on enter press, checks the word entered by the player against a list of all the words that are currently on the board
  * if there is a match, the destroy() function runs to destroy the word on the scroll and also runs a function to call a boom sprite as well as runs function to call a boom sound
  * adds 5 points to the score counter as well as adds one to the correct word counter

#### Areas of Success (Code, Organization)

* Extremely Clean, Easy to Understand Code
  * You have so many helpful comments as to what you are doing along the way.  Even though I don't understand Phaser completely, I could understand the steps you were taking.  Also, very clean with spacing and no redundency.  I also like that you split your code into different documents for different game stages.
* Liked your way of checking for if there were three correct words typed in to add time to the counter
  * Thought it was great to have a counter for correct words and when it hit three, to add time to the time counter as well as reset the correct word counter back to 0.  Super simple and logical.

#### Areas for Improvement (Code, Organization)

* It would be great to have a way to record your score
  * You mentioned this in your to do next things, but I think you are right.  It would be great to have a way to record  your score and see if you are improving.
* Better word choices
  * You already mentioned this in your things you want to do for your game as well.  As you know, there are some not so PC words that come up.  Also, are some of them real words at all?  I will say though that having words like the ones in the game did make it harder because I'm not used to seeing them or knowing their spelling and the muscle memory of typing them was not in my body.

## Additional Notes

Super nice job!  I definitely want to have you explain to me some of the syntax for the Phaser stuff.  Like I said, really neat and clean and easy to follow and understand.  (Is a good example of what you wrote about in your branding statement).  I know you think that the menu looks dumb.  I don't think it is that bad.  I honestly think you just need to do a couple tweeks and it'll look fine.  Add some different fonts, maybe find a slightly different background for behind the scrolling part,  line up the red text a little differently.  Maybe play with trying to fill up some of the "white space" on the sides?  Try the text there? (however I do like the text over the graphic)  Oh, and also get the scrolling div to start at the top of the page.  Really nice job!
