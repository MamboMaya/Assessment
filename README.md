## Scope, hoisting and compartmentalization

### Answer the following:
In you own words, explain the concepts of scope, hoisting, compartmentalization.
Scope deals with the global and local variables. This will determine which variables can be used in a given time in your code.
Hoisting is the compiler rearranging your code to declare certain variables in order to avoid Type Errors.
Compartmentalization is separating the areas and names of your code to make it more readable AND functional.

### Provide examples for all three, below:

#### Scope:
var x = 5

function() {
  var x = 10
  console.log(x)
}

console.log(x)

The two console.log(x) will bring back different values because they are not in the same scope.
#### Hoisting:

function() {
  x = x + 5
  var x = 3
}

Because var x is not defined before it is used in the function, hoisting relocated the declaration to the top of the function to avoid Type Errors.

#### Compartmentalization:
var firstName = "Will"
var lastName = "Hunting"

function greeting() {

  return "Helllooooo " + firstName + " " + lastName + "!"
}
console.log(greeting())


Separation of variables and functions allow the user and other readers to easily move through the code blocks.
