# Code Review for KEXP Live Playlist

## Project Repo

https://github.com/mullfuchs/liveplaylist

## Review

#### Project Purpose

Allow streaming of KEXP radio station and favoriting of current and recent songs.

#### Project Organization

#### Features

* Site streams KEXP radio station
  * Built in player to stream station
* Allows current and favorite songs to favorited
  * Data scraps KEXP site for listing of most recent song and list with abitlty to favorite them.
* Account creation and login to save favorites.
  * Explanation on how it's implemented

#### Areas of Success (Code, Organization)

* Overall layout is logical and user friendly
  * Simple to find things and for the most part make sense where they are.
* Code, functions, and files are named well.
	* Naming is logical and code is well laid out.

#### Areas for Improvement (Code, Organization)

* Would like to see the music to continue streaming as you move to different parts of the site.
  * Could be done with a partial or having the player in a popup window.
* "recent favs go here" list does not clear when user logs out.
  * Remove ability to fave when not logged in? Possibly make that entire div require user to be logged in to either use or see
* Site is very bootstrap looking.
	* Less round corners. More CSS

## Additional Notes

Great concept and much needed.
