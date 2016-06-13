# Code Review for Reno M.

## Project Repo

https://github.com/darkenvy/DungeonTreasure

## Review

The code is modularized and DRY to my inexperienced eye. Many variables are declared throughout the main JS source folder, called "js." These JS files are named appropriately. They are called control.js, hud.js, main.js, and region.js. Reno limited the scope of variables by separating concerns and breaking up chunks of the JS into these distinct files.

In main.js there are many variables declared pertaining land generation, physics, and player stats. The variable names are semantic.

I was somewhat confused by the name of a specific project folder at first. I saw that some of the vendor plug-ins/dependencies were in the "test" project folder. Upon further inspection, it looks like these were different tests checking if Phaser and Perlin were playing nice together. "Test" is a good name for this folder after all.


#### Project Purpose

Create a game using JavaScript, HTML, CSS, and other technology to show what you've learned.

Reno made a Rogue-Like Dungeon Crawler. The player character needs to drive as far down in to the planet while conserving energy, avoiding enemies, and gather supplies.

#### Project Organization

The project organization is well done. It's necessary for a project this large and Reno did a great job commenting and naming his main JavaScript files.

#### Features

* How To Play Pop-up
  * Used a modal that explains the game rules and point of the game
* Random land generation
  * Used a JS plug-in to generate a random set of integers which he transformed in to chunks of land- awesome
* Character movement
  * Used control flow and other checks to get the X and Y position of the player character sprite to change along with the sprite itself
* Hit Detection
  * Implimented Phaser Arcade Physics... ".collide"
  * Allowed enemy creatures to avoid hit detection vs one another

#### Areas of Success (Code, Organization)

* Code Organization
  * Strong point, necesarry for a project of this size.


* Used Interesting Tech
  * I find the use of the Perlin noise generator to be very interesting. I will definitely employ it in the future if I make a game that calls for random land generation, and I'll have the benefit of having this code as an example.




