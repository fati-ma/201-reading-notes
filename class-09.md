# Forms and Events
#### Read: 09 submission 

#### Hello, This is Fatima. You can view my webpage using the following [link](https://fati-ma.github.io/201-reading-notes/class-09)
#### You can go back to the [home](https://fati-ma.github.io/201-reading-notes/) page.

#### In this blog I will give a summary for the chapters 7 and 14 of the book: "HTML & CSS" and chapter 6 from the book "Javascript and Jquery" :books: 

- [x] *Chapter 7: Forms* ✔️
- [x] *Chapter 14: Lists, Tables & Forms* ✔️
- [x] *Chapter 6: Events* ✔️


##### Note: Keywords are emphasised.


## Chapter 7: Forms

### Why we need them:

In addition to *enabling users to search*, forms also allow users to *perform other functions online*. Forms are used when registering as a member of a website, when shopping online, and when signing up for newsletters or mailing lists.

#### There are several types of form controls that are used to collect information from visitors to sites.

1. Adding Text:
   - Text input (single-line)
   - Password input
   - Text area (multi-line)
   
2. Making Choices:
   - Radio buttons
   - Checkboxes
   - Drop-down boxes 
   
3. Submitting Forms:
   - Submit buttons
   - Image buttons
   
4. Uploading Files:
   - File upload
   
### How Forms Work

1. A user fills in a form and then presses a button
to submit the information to the server.

2. The name of each form
control is sent to the
server along with the
value the user enters or
selects.

3. The server processes
the information using a
programming language
such as PHP, C#, VB.net,
or Java. It may also store
the information in a
database.

4. The server creates a new
page to send back to the
browser based on the
information received.

### Form Structure

`<form>` Form controls live inside a
<form> element. This element
should always carry the action
attribute and will usually have a
method and id attribute too.
  
`action` Every <form> element requires
an action attribute. Its value
is the URL for the page on the
server that will receive the
information in the form when it
is submitted.
  
`method`
Forms can be sent using one of
two methods: `get` or `post`. 

`id` 

### Text Input

`<input>`  used
to create several different form
controls. The value of the type
attribute determines what kind
of input they will be creating.

`type="text"` When the type attribute has a
value of text, it creates a singleline text input.

`name` into a form, the server needs to
know which form control each
piece of data was entered into. 

`size` The size attribute should not
be used on new forms. It was
used in older forms to indicate
the width of the text input 

`maxlength`  to limit the number
of characters a user may enter
into the text field.

### Password Input

`<input>`

`type="password"` When the type attribute has
a value of password it creates
a text box that acts just like a
single-line text input, except
the characters are blocked out. 

`name` The name attribute indicates
the name of the password input,
which is sent to the server with
the password the user enters.

`size` `maxlength` It can also carry the size and
maxlength attributes like the
the single-line text input.

### Text Area

`<textarea>` used to create a mutli-line
text input


### Radio Button and Checkbox

`<input>`  `type="radio"` `type="checkbox"` `name` 

`value` the value that is sent to the
server for the selected option.
The value of each of the buttons
in a group should be different.

`checked` used to indicate which value (if
any) should be selected when
the page loads. 

### Drop Down List Box

`<select>`  used
to create a drop down list box. It
contains two or more `<option>`
elements. 

```
<select name="devices">
 <option value="ipod">iPod</option>
 <option value="radio">Radio</option>
 <option value="computer">Computer</option>
</select>
```

### Multiple Select Box

```
<select name="instruments" size="3"
 multiple="multiple">
 <option value="guitar" selected="selected">
 Guitar</option>
 <option value="drums">Drums</option>
 <option value="keyboard"
 selected="selected">Keyboard</option>
 <option value="bass">Bass</option>
</select>
```

### File Input Box

`<input>`  `type="file"`

### Submit Button and Image Button

`<input>` `type="submit"` `type="image"`


## Chapter 14: Lists, Tables & Forms

### Lists

`list-style-type` 

`list-style-image`

`list-style-position`

`list-style`


### Tables

`width` `padding` `text-transform` `letter-spacing, font-size` `border-top, border-bottom` `text-align` `background-color` `:hover`

`empty-cells` `border-spacing` `border-collapse` 


### Forms

#### Styling text input

`font-size` `color` `background-color` `border` `border-radius` 
` :focus` `:hover` `background-image`

#### Kye points:
- Forms are easier to use if the form controls are
vertically aligned using CSS.

- Forms benefit from styles that make them feel more
interactive.


## Chapter 6: Events

HTML events are "things" that happen to HTML elements.
When JavaScript is used in HTML pages, JavaScript can "react" on these events.

![event](/events.jpg)




















 












