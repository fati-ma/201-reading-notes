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

#### Calculate daily Likes

Popularity of a video is measured in Likes. And the formula for calculating Likes is the number of viewers times the percentage of viewers who'll Like a video. In other words, **viewers times percentage**.

To calculate the number of viewers per day, generate a **random number between 10 and 30** and then multiply it by the epic rating of that video.

The **percentage** of viewers who'll Like a video depends on whether or not the video contains animals.

```
EpicFailVideo.prototype.generateRandom = function(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

EpicFailVideo.prototype.dailyLikes = function() {
  var viewers, percentage;

  viewers = this.generateRandom(10, 30) * this.epicRating;

  if (this.hasAnimals) {
    percentage = 0.75;
  } else {
    percentage = 0.40;
  }

  return Math.round(viewers * percentage);
}
```

#### Calculate weekly Likes

```
EpicFailVideo.prototype.weeklyLikes = function() {
  var total = 0;

  for (var i = 0; i < 7; i++) {
    total += this.dailyLikes();
  }

  return total;
}
```


## Chapter 6: Tables

A **table** represents information in a *grid format*. 
Each block in the grid is referred to as a **table cell**.

### Basic Table Structure `<table>`  `<tr>`  `<td>`

- The `<table>` element is used to create a table.
- `<tr>` stands for table row.
- Each cell of a table is represented using a `<td>`element. (The td stands for table data.)
- `<th>` to represent the heading for either a column or a row. (The th stands for table heading.) 
- The `colspan` and `rowspan` attributes can be used on a <th> or <td> element and indicates how many columns or rows that cell should run across.
- `<thead>` The headings of the table should sit inside the <thead> element.
- `<tbody>` The body should sit inside the <tbody> element.
- `<tfoot>` The footer belongs inside the <tfoot> element. 
  
![table](https://learn.winona.edu/w/images/3/3a/Tbl_Example.jpg)  


## Chapter 3: Functions, Methods, and Objects


### Creating a JavaScript Object

```
var person = {
  firstName: "John",
  lastName : "Doe",
  id       : 5566,
  fullName : function() {
    return this.firstName + " " + this.lastName;
  }
};
```

#### Object Construct

```
function Person(first, last, age, eye) {
  this.firstName = first;
  this.lastName = last;
  this.age = age;
  this.eyeColor = eye;
}
```

Creating new object and calling it:

```
var myFather = new Person("John", "Doe", 50, "blue");
var myMother = new Person("Sally", "Rally", 48, "green");
```

#### The (this) Keyword

In JavaScript, the thing called **this** is the object that "owns" the code.
The value of this, when used in an object, is *the object itself*.


#### Arrays are objects

**An Object**

```
costs = {
   room1: 420,
   room2: 460
   };
```

**An Array**

```
costs = [420, 460];
```


#### Arrays in an object and Objects in an Array

![objarr](https://miro.medium.com/max/470/1*oNiNLXLML6i0kknHkOGArQ.png)


#### Three groups of built-in objects

1. Browser object model

![bow](https://static.javatpoint.com/images/javascript/bom.jpg)


2. Document object model

![doc](https://www.w3schools.com/js/pic_htmltree.gif)


3. Global javascript objects
   - String
   - Number
   - Boolean
   - Date
   - Math
   - Regex

#### Creating an instance of the Date object

```
var today = new Date() ;
```

## Summary

- Web browsers implement **objects** that represent both the browser window and the document loaded into the browser window.

- JavaScript has several **built-in objects** such as String, Number, Math, and Date. Their *properties and methods* offer functionality that help write scripts.

- **Arrays** and **objects** can be used to create complex data sets. 

