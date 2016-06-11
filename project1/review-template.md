Code Review for Ryan Rotz

Project Repo 

https://github.com/ryanrotz/name-that-emotion

Review

Project Purpose

This projects purpose is to help children with Autism practice identifying facial expressions and body language and identify the corresponding emotion.

Project Organization

Features

-Displays a multiple choice question, and a photo conveying an emotion
  The user clicks on the start game button, which causes a photo and four answer choice buttons to appear.
  The event listener on the button calls a function to change the inner HTML of a div, showing the picture.
-Displays a modal after selecting an answer, letting the user know of a right or wrong answer
  The user clicks on an answer button and is shown a modal that displays a message corresponding to the correctness of the answer chosen, as well as a button that takes them to the next question if they submitted a correct answer, causing the score to increase.
  The event listeners on the answer buttons cause the value of the correct answer and the value tied to each button to be compared to check for correctness, displaying a message. If the values match, the score is increased by 10.
-Displays a winning message
  Once enough correct answers have been submitted, thus shorteneing the array of answer objects, a message is displayed letting the user know that they have completed level one.

Areas of Success (Code, Organization)

-Good use of semantic markup
  The functions are named based on their function(play, reset, start, etc.), as well as other variables being named based on their relationship to the flow of the game.
-Good use of responsive CSS styling
  The page displays well when the screen size is adjusted, nothing seems to dissapear or overlap with other elements.

Areas for Improvement (Code, Organization)

-Code could be cleaned up a little
  There a a couple of instances of extra white space, as well as some comments that could probably be removed. There are also some commented out and seemingly unused CSS properties that might as well be removed if they don't serve a purpose
-Possibility of implementing a contructor
  You might be able to make things just a little more DRY by using a contructor.

Additional Notes

Your page looks good Ryan, well done on the CSS especially. Maybe when you come back to this project some day, you'll get those extra levels added in. A job well done.
