# HTML Links, CSS Layout, JS Functions
#### Read: 04 submission 

#### Hello, This is Fatima. You can view my Markdown webpage using the following [link](https://fati-ma.github.io/201-reading-notes/class-04)
#### You can go back to the [home](https://fati-ma.github.io/201-reading-notes/) page.

#### In this blog I will give a summary for the chapters 4 and 15 of the book: "HTML & CSS" and for chapter 3 from the book: "Javascript and Jquery" :books: and for this [article](https://www.codefellows.org/blog/6-reasons-for-pair-programming/):  :

- [x] *Chapter 4: Links* ✔️
- [x] *Chapter 15: Layout* ✔️
- [x] *Chapter 3: Functions, Methods, and Objects* ✔️
- [x] *Chapter 4: Article: 6 Reasons for Pair Programming* ✔️


##### Note: Keywords are emphasised.


## Chapter 4: Links

- ***Links*** are created using the `<a>` element.
- The `<a>` element uses the `href` attribute to ***indicate the page we are linking to***.
- If we are linking to a page within our own site, it is best to use ***relative links*** rather than qualified ***URLs***.
- We can create links to open email programs with an email address in the "to" field.
- We can use the `id` attribute to target elements within a page that can be linked to.

![links](https://lh3.googleusercontent.com/proxy/zlJifL7TozvV2IiKi9nSMI0I_QV7A4hiMYR2FKgu5zsanbaaUZBQp1JGB20iSW2ED4Ub_A1s0xOryE7hw3iVTVYM1IF9-7sr6oqE9-qaQE6JPqZkODZ4vkoSxXYMOUwGq11Y6UClyvs5U9UnzuI_rADpVVpoLTI0NTCiKP4r)


#### Keywords:

`<a>` Links are created using the <a> element which has an attribute called href. The value of the href attribute is the page that you want people to go to when they click on the link.
  
`Absolute URL` When you link to a different website, the value of the `href` attribute will be the full web address for the site.

`Relative URL` When you are linking to other pages within the same site.

`Directories` Folders on a website. 

`mailto: ` To create a link that starts up the user's email program and addresses an email to a specified email address.

`target` If I want a link to open in a new window.



## Chapter 15: Layout


#### Key Concepts in Positioning Elements

1. **Building Blocks**:
   - `Block-level` elements start on a new line
   - `Inline elements` flow in between surrounding text
   
2. **Containing Elements**: If one block-level element sits *inside* another block-level element then the **outer box** is known as the **containing or parent element**.  


### Position property in CSS

#### Kyewords:

`position:static`: default

`position:relative`: moves an element in relation to where it would have been in normal flow.

`position:absolute`: the box is taken out of normal flow and no longer affects the
position of other elements on the page. 

`position:fixed`:  a type of absolute positioning that requires the position property
to have a value of fixed


![pos](https://s3.amazonaws.com/viking_education/web_development/web_app_eng/css_positioning_absolute_relative_fixed.png)


`z-index`: to control which element sits on top.

`float`: to take an element in normal flow and place it as far to the left or right of the containing element as possible.

`clear`: to say that no element (within the same containing element)
should touch the left or righthand sides of a box. 

`Resolution` refers to the number of dots a screen shows per inch.

`Fixed width` layout: designs do not change size as the user increases or decreases
the size of their browser window. Measurements tend to be given in pixels.

`Liquid` layout designs: stretch and contract as the user increases or decreases the
size of their browser window. They tend to use percentages.

`Grid`:  the placement or arrangement of visual elements.



## Chapter 3: Functions, Methods, and Objects

***Functions*** let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of statements). 

![func](https://s3.ap-south-1.amazonaws.com/s3.studytonight.com/tutorials/uploads/pictures/1587882057-1.png)

```
function getSize (width, height, depth) {
  var area = width * height;
  var volume = width * height * depth;
  var sizes= [area , volume];
  return sizes;
}
var areaOne = getSize (3, 2, 3)[0];
var volumeOne = getSize (3, 2, 3)[1]; 
```

### Immediately invoked functions

```
var area = (function(){
var width = 3;
var height = 2;
return width * height;
} () );
```



## Article: 6 Reasons for Pair Programming

***Pair programming*** commonly involves two roles: the **Driver** and the **Navigator**. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs.

Pair programming leads to:
1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness





