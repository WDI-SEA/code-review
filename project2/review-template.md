# Code Review for the Man, the Myth, the Legend - Reno "@darkenvy" McDonald

## Squidl.ink

https://github.com/darkenvy/Squidl.ink
http://squidl.ink

## Review

#### Project Purpose

The purpose of this app is to let users share files without uploading them to the cloud, ala DropBox. Users drag and drop a file into the page, creating a private link they can share with anyone they want to share their file(s) with.

#### Project Organization

#### Features

* Modal explaining how app works (/public/js/page-global.js ln:30)
  * If it's the user's first visit to the site, show sweet alert titled "What is Squidlink?".

* Drag and drop files to create share-able links (/public/js/page-global.js ln:149)
  * Honestly, Reno's code is hard-ish for me to read, here. Not sure what the class "dragging" is doing, but I'm thinking it's CSS-related. On line 185 he declares var file = dataTransfer.files[0], or first item in "dataTransfer", checks to see if it's over 1GB (and if so, sends a warning), and then calls function seed(), passing in var file. I think Reno's code is above my pay-grade, LOL. :-)

* Streaming or downloading the file (/public/js/page-download.js ln: 3)
  * After clicking the link shared with you, you are given the option of downloading the file, or stream and download it. If you choose to stream, it will set "playMedia" to true, and then run the streamOrDownload function (ln: 23), which hides/unhides some elements (by adding or removing Class 'hide), and calls the download() function, passing in the var hash, which he's set to the value of the download button.

#### Areas of Success (Code, Organization)

* Awesome Sauce
  * This is a bad-ass project, and it raises my already high-esteem for Reno, his intelligence, and his coding abilities.
* Above my Pay-Grade
  * Without poring over this code for a few hours or checking documentation, I have no clue about some of what he's doing. I'm simultaneously impressed, AND bringing dishonor to my family.

#### Areas for Improvement (Code, Organization)

* Commenting for laypeople
  * There are several great comments throughout, but not enough for me to fully Grok what was going on in some spots.

* That's it. Only one area for improvement that this dude could see :-)

## Additional Notes

Reno, you're awesome. If I weren't straight, I would totally be so smitten with you right now, LOL  High five buddy! You did a really great job!!  -Josh McBroom
