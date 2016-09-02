# Code Review for Jamie Karlovich

## Project Repo

web: https://nightynight.herokuapp.com/
Git:https://github.com/jkarlovich/NightyNight/

## Review

#### Project Purpose

The purpose of this project is to create a night on the town based on a performance you are interested in attenting. The client gets inspiration on where to eat and grab a drink near their show. The client also has a link to buy show tickets.

#### Components
* APIs used: 
  * 'http://api.eventful.com/json/events/search'
  * 'https://maps.googleapis.com/maps/api/place/nearbysearch/json'
* Boostrap and flexbox/custom css
* jQuery tricks
* 3 controllers and main ejs views
* Login/out functionality

#### Project Organization

#### Features

* Search for a show by keyword/phrase
  * Entered search term on the home page form redirects you to a results page where an api call is done restriced by the search term entered.
* See event description and nearby restaurants
  * When you click on a result, you are taken to a detail page. The detail page does another request to the api and limits results based on the even selected. The google api is then called using the lat/long from the event details in the first api and restricts by keyword 'restaurant' and ranks results by distance.
  * The event details and description appears on the left and a map appears on the right with the show location as a flag and nearly restaurant POIs(points of interest). The POIs are listed underthe map and event details. You can click on a POI to show you the name and address.
* Buy > Save a show to your favs/profile
  * A button on the details page will save your event if you are logged in. The show name and postal code location are saved in a list for the client to retrieve later. 
  * You can also delete shows frm this list. Feature in progress > You can click on the event url for more details which opens in a different tab . 

#### Areas of Success (Code, Organization)

* Header, footer and homepage
  * The header and footer were well styled and informative. I liked the bold hover-over color when i was selecting. The tranparant background over the picture was genious.
* Website layout
  * The layout was easy to use and digest, I  had no trouble navigating and seeing the info i needed. I liked the detail page format.
* Jquery, focus on field, open new tab
  * I liked the use of jQuery. Even if it was not althe way complete, i think it was great to use focus on a text field, and open a new tab! Small things that are very classy and user friendly.


#### Areas for Improvement (Code, Organization)

* Login and signup modal vs. page
  * I noticed there is a login page and a login modal. When I clicked 'Buy' I got to the login page instead of the modal, but I could still open the modal. I was unable to signup however, the route to signup was missing a forward slash in the route (this happened to us a few times before!)
* Event search not very specific
  * It looks like the api wasn't very structured unfortunately, but it would have been nice to reduce the search results by Seattle or my location in addition to key word. I noticed some volunteer events as well, it would have been nice to restrict by category to keep to the 'night out' theme.
* The color palette was a little inconsitant through the site, black, purple, green. Sometimes the coloring would take away from the content i was trying to view
  * I liked the color choices individually, but maybe stick to a theme throught the website for flow. I think more white space would have made it easier to read some of the content as well.

## Additional Notes

Beautiful site! I liked that it was easy to navigate and use as a client. Hopefully your next api will be easier to work with!
