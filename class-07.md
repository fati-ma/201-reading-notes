# HTML Tables; JS Constructor Functions
#### Read: 07 submission (Object-Oriented Programming)

#### Hello, This is Fatima. You can view my Markdown webpage using the following [link](https://fati-ma.github.io/201-reading-notes/class-07)
#### You can go back to the [home](https://fati-ma.github.io/201-reading-notes/) page.

#### In this blog I will give a summary for the [reading topic](https://github.com/codefellows/domain_modeling#domain-modeling) and the chapter 6 of the book:"HTML and CSS" and  chapter 3 of the book: "Javascript and Jquery" :books: 


- [x] *Topic: Domain Modeling* ✔️
- [x] *Chapter 6: Tables* ✔️
- [x] *Chapter 3: Functions, Methods, and Objects* ✔️


##### Note: Keywords are emphasised.


## Topic: Domain Modeling

***Domain modeling*** is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an **object-oriented** model.

### Model epic fails videos

Two essential metrics for gauging popularity are an **epic rating** and **whether or not the video has animals**.
Build self-contained objects with the same attributes and behaviors.

#### Define a constructor and initialize properties

Use a **constructor function**.


| Property      | Data | Type     |
| :---:        |    :----:   |          :---: |
| epicRating      | 1 to 10       | Number   |
| hasAnimals   | true or false        | Boolean      |


Here's an implementation of the `EpicFailVideo` constructor function.

```
var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail);
console.log(corgiFail);
```

This is **object-oriented programming** in JavaScript at its most fundamental level.

The `new` keyword instantiates (i.e. creates) an object.
The **constructor function** initializes properties inside that object using the this variable.
The **object** is stored in a variable for later use.

#### Generate random numbers

JavaScript standard library includes a `Math.random()` function for a random number generating.

```
EpicFailVideo.prototype.generateRandom = function(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}
```
