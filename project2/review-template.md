# Code Review for story-syntax Chris Madison

## Project Repo

_Put the link to your partner's project here_
  * https://github.com/CMadison/story-syntax

## Review

#### Project Purpose

_List the purpose and components of the project here_
  **Purpose__

  * The purpose is to have a site for people who are new to creating
  * user stories, to be able to go to sign up and quickly be able to 
  * create and understand the layout and flow of a user story.

  **Components
    *clean well designed layout 
    *user sign up && facebook oAuth
    *creating users and the user story's
    *saving user storys and the ability to edit them and delete them


#### Project Organization

#### Features

* Feature 1
  * Explanation on how it's implemented

    -Facebook OAuth-

      - implemented the facebook oauth using passport-facebook module.
        using the facebook api it grabs the users email and find or creates a user
        with email, facebook id as the user id and the facebook access token
        for authentication.

* Feature 2
  * Explanation on how it's implemented

    - User ability to Edit and Delete user stories

      - For the edit GET route Chris takes the req.params and uses the id
        of the specific story and grabs the story from the database and puts
        the current content into the correct form fields for easy updating.

      - For the delete route Chris uses the POST route to grab the specific
        story id search the database and delete the coresponding story
        then redirects you back to the page to see its been deleted

* Feature 3
  * Explanation on how it's implemented

    - styling

      - it looks like he implemented a good bootstrap template and fitted it
        for his needs. Setting up his content in a clean way and making the page
        easy to navigate and use.

#### Areas of Success (Code, Organization)

* Attribute 1
  * Explanation on why you found it successful or elegant

    - I am super impressed with the styling and layout of the app.
      Everything flows nicely and is easy to use.

* Attribute 2
  * Explanation on why you found it successful or elegant

#### Areas for Improvement (Code, Organization)

* Attribute 1
  * Explanation on how it could be improved

    - I noticed that when a user try's to create a story without being signed
      in it lets you create the story and stores it in the database, then when 
      you click submit it prompts you to log in. When you sign up or log in the
      story you created shows up.

    - It would be better if the form fields stay filled in when your prompted to
      sign up and then you could re-submit the story. And it prevented you from
      creating the story in the database until you were fully logged in.

* Attribute 2
  * Explanation on how it could be improved

    - with the edit and delete routes instead of using GET and POST routes
      it would be better to use ajax and do PUT and DELETE methods

## Additional Notes

_Place any additional notes here_

I enjoyed the 404 easter egg..