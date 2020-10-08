# JS Object Literals; The DOM
#### Read: 06 submission 

#### Hello, This is Fatima. You can view my Markdown webpage using the following [link](https://fati-ma.github.io/201-reading-notes/class-06)
#### You can go back to the [home](https://fati-ma.github.io/201-reading-notes/) page.

#### In this blog I will give a summary for the [reading article](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming) and the chapters 3 and 12 of the book: "Javascript and Jquery" :books: 


- [x] *Article: Understanding The Problem Domain Is The Hardest Part Of Programming* ✔️
- [x] *Chapter 3: Object Literals* ✔️
- [x] *Chapter 5: Document Object Model* ✔️


##### Note: Keywords are emphasised.


## Article: Understanding The Problem Domain Is The Hardest Part Of Programming


The author believes that the hardest thing about programming is learning the problem domain.
The he explained from his perspective why problem domain is difficult, because the real world is a messy place.  Many of the problem domains programmers face are difficult to understand and look completely different depending on their viewpoint.
If understanding the problem domain is the hardest part of programming and the programmar wants to make programming easier, they can do one of two things:
1.Make the problem domain easier
2.Get better at understanding the problem domain
>It is easy to fall into the trap of thinking you understand enough of the problem to get started coding it. 



## Chapter 3: Object Literals


***Objects*** group together a *set of variables and functions* to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on *new names*. 


- IN AN OBJECT: VARIABLES BECOME
KNOWN AS **PROPERTIES** 


- IN AN OBJECT: FUNCTIONS BECOME
KNOWN AS **METHODS**


- In an object,
the name is called a **key**.


```
var person = {
  firstName: "John",
  lastName: "Doe",
  age: 50,
  eyeColor: "blue"
};
```

##### An object literal is a list of name:value pairs (like age:50) inside curly braces {}.


#### Accessing Object


``` 
objectName.propertyName
```
or
```
objectName["propertyName"]
```


## Chapter 5: 


As a browser loads a web page, it creates a model of that page.
The model is called a ***DOM tree***, and it is stored in the browsers' memory.
It consists of four main types of nodes. 
1. THE DOCUMENT NODE
2. ELEMENT NODES 
3. ATTRIBUTE NODES 
4. TEXT NODES 

![dom](https://www.w3schools.com/js/pic_htmltree.gif)


### WORKING WITH THE DOM TREE 

Accessing and updating the DOM tree involves two steps:
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes. 


![get](https://www.oreilly.com/library/view/head-first-html5/9781449314712/httpatomoreillycomsourceoreillyimages2224176.png.jpg)


### The item() method and Array sentax


**There are two ways to select an element from a Nodelist:
The item() method and array syntax. **

```
var elements = document.getElementsByClassName('hot')
if (elements.length>= 1) {
   var firstltem = elements.item(O);
} 
```
or
```
var elements = document.getElementsByClassName('hot')
if (elements.length>= 1) {
   var firstltem = elements[0];
} 
```


### Selecting elements by tag name

```
var elements = document.getElementsByTagName('li '); //I Find <li> elements
if (elements.length> O) {
  var el = elements[O];
  el.className = 'cool';
}
```


### Repeating actions

```
var hotlt ems = document .querySelectorAl l (' l i . hot') ; 

if (hot ltems.length > O) {

   for (var i=O; i<hotl tems.length; i++) { 
      hotltems[i] .className = 'cool';
   }
}
```

### Key points:

- The browser represents the page using a **DOM tree**.

- DOM trees have four types of **nodes: document nodes, element nodes, attribute nodes, and text nodes**.

- You can **select element nodes** by their **id** or **class**
attributes, by **tag** name, or using **CSS selector** syntax.

- Whenever a DOM query can return more than one
node, it will **always return a NodeList**.

- From an element node, you can access and update its
content using properties such as textContent and
innerHTML or using DOM manipulation techniques.

- An element node can contain multiple text nodes and
**child elements** that are siblings of each other.

- In older browsers, implementation of the DOM is
inconsistent (and is a popular reason for using jQuery).
Browsers offer tools for viewing the DOM tree . 


