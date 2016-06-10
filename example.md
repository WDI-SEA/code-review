# Code Review for Brian Hague

## Project Repo

https://github.com/WDI-SEA/temperature-converter-dom/tree/brian-finished

## Review

#### Project Purpose

The purpose of the project is to convert a temperature from Fahrenheit to Celsius.

#### Project Organization

#### Features

* Convert a Fahrenheit temperature to Celsius
  * A user has an input field and a button available to click. The user can enter a number into the input field and submit the form. Once submitted, the user can see the converted temperature.
  * The logic was implemented by attaching an event listener to the form, converting the temperature, and appending the temperature to the DOM.

#### Areas of Success (Code, Organization)

* Variables are named very well
  * The form, temperature, and output variables are named well, and it's easy to understand what the variables are storing.
* Simplicity in the DOM
  * The HTML elements are well-indented and organized.

#### Areas for Improvement (Code, Organization)

* Conversion is arbitrary to the user
  * The HTML never tells the user what temperature you're converting to, which can be a UX issue.
  * The code to convert the temperature is also hard to understand. Perhaps creating a function called `convertFahrenheitToCelsius` would make it easier to see that we're converting the temperature to Celsius.
* Missing CSS
  * This page could be styled a lot better. There's no CSS.

## Additional Notes

Nice job!
