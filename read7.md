# DOMAIN MODELING

The process of creating a conceptual model in code for a specific problem.

Object oriente model: an entity that stores data in properties and closes behaviors in methods.

1. `new` keyword creates an object
2. the constructor function initializes properties inside that object using `.this` variable
3. the object is stored in a variable for later use

ex.)

```
let bestCities = function(bestFood, bestLife) {
  this.bestFood = bestFood;
  this.bestLife = bestLife;
}

let goodChinese = new bestCities(8, false)
let goodAir = new bestCities(2, true)

console.log(goodChinese);
console.log(goodAir);
```

## GENERATE RANDOM NUMBERS
`Math.random()`

ex.)
```
let bestCities = function(bestFood, bestLife) {
  this.bestFood = bestFood;
  this.bestLife = bestLife;
}

bestCities.prototype.generateRandom = function(min, max){
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

let goodChinese = new bestCities(8, false)
let goodAir = new bestCities(2, true)

console.log(goodChinese);
console.log(goodAir);
```

## CALCULATE DAILY LIKES
ex.)
```
let bestCities = function(bestFood, bestLife) {
  this.bestFood = bestFood;
  this.bestLife = bestLife;
}

bestCities.prototype.generateRandom = function(min, max){
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

bestCities.prototype.dailyLikes = function() {
  let viewrs, percentage;

  viewers = this.generateRandom(10, 30) * this.bestFood;

  if (this.bestLife){
    percentage = 0.75;
  } else {
    percentage = 0.40;
  }
  return Math.round(viewers * percentage);
}

let goodChinese = new bestCities(8, false)
let goodAir = new bestCities(2, true)

console.log(goodChinese);
console.log(goodAir);
```

## CALCULATE WEEKLY LIKES


ex.)
```
let bestCities = function(bestFood, bestLife) {
  this.bestFood = bestFood;
  this.bestLife = bestLife;
}

bestCities.prototype.generateRandom = function(min, max){
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

bestCities.prototype.dailyLikes = function() {
  let viewrs, percentage;

  viewers = this.generateRandom(10, 30) * this.bestFood;

  if (this.bestLife){
    percentage = 0.75;
  } else {
    percentage = 0.40;
  }
  return Math.round(viewers * percentage);
}

bestCities.prototype.weeklyLikes = function(){
  let total = 0;

  for (let i = 0; i < 8; i++) {
    total += this.dailyLikes();
  }
  return total;
}

let goodChinese = new bestCities(8, false)
let goodAir = new bestCities(2, true)

console.log(goodChinese);
console.log(goodAir);


```

## DOMAIN MODELING TIPS
- A single entity that has many instances, use self-contained objects with the same behaviors and attributes
- Model its attributes w/ a constructor function that initializes properties
- Model the behaviors with small methods doing a small job efficiently 
- create instances using `new` keyword and call the constructor function
- store the new object in a variable so you can access it later on the *outside*
- use `.this` within methods so you can access object properties from the *inside*

# Chapter 6: TABLES (HTML & CSS)

Table: represents info in a grid format.

`<table>` element creates a table

`<tr>` is a row

`<td>` is all the table data

# Chapter 3: FUNCTIONS, METHODS, AND OBJECTS (JAVASCRIPT)
## Functions

## Methods

## Objects

Literal notation

ex.)
properties
```
var dude = {
  name: Sam;
  age: 62
  mindsetage: 15
}
```
method
ex.)
```
sayHi: function( {
  return this.age - this.mindsetage;
};
```

Accesing an object with dot notation
```
var dudeName = dude.name;
var howOld = dude.getAge;

You can also access properties with [''] instead of just fe. .name
```

Global context/scope = when a function is craeted at the top level of a script.

Local = inside

## ARRAYS IN AN OBJECT
ex.)
`costs.room1[0];`

## OBECTS IN AN ARRAY
ex.)
`costs[2].phone;`

1. BOM (Browser Object Model)
- creates model of browser tab or window
2. DOM (Document Object Model)
- Creates model of curent webpage
3. GJO (Global javascript Objects)
- group of individual objects that realte to different parts of Javascript

[<==ReturnToHome](README.md)