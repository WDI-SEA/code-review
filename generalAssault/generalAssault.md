# Code Review for _Insert Name Here_

## Project Repo

https://github.com/dropTheNon/WDI-Project-1

## Review

#### Project Purpose

This game is similar to risk, and the purpose was to test and leverage the knowledge we've gained over the past couple weeks to build a game.

A turn-based strategy game using dice. Players deploy armies, attack nearby territories, and advance troops to conquered territories, with the goal being to eradicate your opponent from the face of the earth! The game ends when one player no longer controls any territories.

#### Project Organization

This project has been setup very similar to most of the class deliverables. The main folder is the source folder which has 3 sub folders (css, images, and js). There is a main index.html file in the src folder for all of the html. The style.css file is in the css folder. This provides all of styling for the site minus the layout portion that is handled by bootstrap.The js folder has one app.js file that houses all of the javascript. The imgaes folder has one image that is referenced in the html for the map.

#### Features

* Dice Roll function
  * This is a dice roll function that is only used in one section of the game. It's used when a player attacks and when a player defends. This is the bit of logic that governs who whins and who loses when a territory gets attacked.

  // Dice roll function
var diceRoll = function() {
  return Math.floor(Math.random() * 6) + 1;
};

// Rolling Dice for each player, pushing into their Array
    for (var i = attackerDiceCount; i > 0; i--) {
      attackerDiceResults.push(diceRoll());
    }
    for (var j = defenderDiceCount; j > 0; j--) {
      defenderDiceResults.push(diceRoll());
    }

* Deploy Troops - Initial
  * This feature is responsible for deploying troops to their territories for the initial start of the game. This is a feature that is governed by the page load, and the user does not have access to control where troops are delploy at the start of a new game.

  var dropFunction = function() {
  numToDrop = numTerritories / totPlayers;
  while (p1Territories.length < (numToDrop - 1)) {
    terrToPush1 = territories[Math.floor(Math.random() * territories.length)];
    if (terrToPush1.player === 'neutral') {
      terrToPush1.player = 'p1';
      p1Territories.push(terrToPush1);
      var p1TerritoriesNames = [];
      for (var i = 0; i < p1Territories.length; i++) {
        p1TerritoriesNames.push(p1Territories[i].name);
      }
    }
  }
  while (p2Territories.length < (numToDrop - 1)) {
    terrToPush2 = territories[Math.floor(Math.random() * territories.length)];
    if (terrToPush2.player === 'neutral') {
      terrToPush2.player = 'p2';
      p2Territories.push(terrToPush2);
      var p2TerritoriesNames = [];
      for (var i = 0; i < p2Territories.length; i++) {
        p2TerritoriesNames.push(p2Territories[i].name);
      }
    }
  }
};

* Advance Troops
  * This feature is responsible for advancing troops to new territories after a new territory has been captured. There are two functions, one to show and hide html elements that accepts user inputs and the actual function that runs the logic once the user has provided the necessary parameters via the html elements.

  // Function to create dropdowns to advance troops
var advanceTroops = function(attTerritory, defTerritory) {
  $('.advanceTroopsSelect').html('<option value="0" disabled selected hidden>How many troops to advance?</option>');
  advanceableTroops = parseInt(attTerritory.troops) - 1;
  if (advanceableTroops > 0) {
    for (var i = 0; i <= advanceableTroops; i++) {
      // var j = i - 1;
      if (turnCount % 2 === 0) {
        $('.advanceTroopsSelect.p1').append("<option value='" + i + "'>" + i + "</option>");
      } else {
        $('.advanceTroopsSelect.p2').append("<option value='" + i + "'>" + i + "</option>");
      }
    }
  }
  advancingTerritory = attTerritory;
  receivingTerritory = defTerritory;
  attackFrom();
};

// Function to actually advance the troops!
var advanceTheTroops = function(advancingTerritory, receivingTerritory, advanceableTroops) {
  console.log(advanceableTroops);
  advancingTerritory.troops = parseInt(advancingTerritory.troops) - parseInt(advanceableTroops);
  console.log(advancingTerritory.troops);
  receivingTerritory.troops = parseInt(receivingTerritory.troops) + parseInt(advanceableTroops);
  whoseTurn();
  console.log(attTerritories);
  console.log(territories);
};

#### Areas of Success (Code, Organization)

* Uses functions well
  * The use of functions throughout this project makes it easy to read, and relatively modular.
* Well commented
  * Useful comments have been placed at the beginning section of each major function.

#### Areas for Improvement (Code, Organization)

* Some of the functions could have been combined into one.
  * Some of the functions create html elements, while another function with a similar name runs the logic on the backend. I'd recommend refactoring these into the same function if time permitted.
* CSS could be prettier
  * Consider making the inputs for player 1 and player 2 the same. This way you'll have less html elements that need to get manipulated.

## Additional Notes

_Place any additional notes here_
