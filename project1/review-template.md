# Code Review for Dan Rasmussen

## Project Repo

http://imdanras.github.io/Baseball-Quiz/?

## Review

#### Project Purpose

The Baseball Quiz. 
A two player multiple choice quiz all about baseball. 


#### The game has has an index directories that contains a .js file and a .css file. 


#### Features

* Feature 1 Start button
  * Starts game and deploys first question into the question div. by utilizing an event listener for the question div. and starts to pull questions from the array.

* Feature 2 Answer buttons
  * There are always four answer buttons. They are each assigned to A, B, C, and D. The correct answer is determined by using this “if” statement that is tailored specific to each of the four buttons.  if (questionsArray[questionCounter].answer === questionsArray[questionCounter].choices[0]) {  
winState = 'correct';
console.log('correct answer B');

* Feature 3 if the answer is correct a Modal is used :
  * $('#myModalLabel').html('You Got it!'); 
$('.modal-body').html(questionsArray[questionCounter].tidbit);

* Feature 4 if anything but the correct answer is click this Modal is called:
  * $('#myModalLabel').html('Nope! Guess Again'); 

*Feature 5 the next button
  * the next button adds the next question, runs the endOfGame function, loads the correct answers, hides the correct answers, and shows the player 1 and 2 button 


#### Areas of Success (Code, Organization)

* Questions array
  * I like how you have all the questions in an array that more questions can easily be added to.
* Organization
  * I also like how all of your code is very organized and seems to be indented in a easy to read format.

#### Areas for Improvement (Code, Organization)

* Comments
  * More comments will help us understand how the game works.
* Responsiveness 
  * Responsiveness could be something to improve on.

## Additional Notes

Nice work!
