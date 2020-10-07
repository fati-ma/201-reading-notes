# HTML Images; CSS Color & Text
#### Read: 05 submission 

#### Hello, This is Fatima. You can view my Markdown webpage using the following [link](https://fati-ma.github.io/201-reading-notes/class-05)
#### You can go back to the [home](https://fati-ma.github.io/201-reading-notes/) page.

#### In this blog I will give a summary for the chapters 5, 11 and 12 of the book: "HTML & CSS" :books: 

- [x] *Chapter 5: Images* ✔️
- [x] *Chapter 11: Color* ✔️
- [x] *Chapter 12: Text* ✔️


##### Note: Keywords are emphasised.


## Chapter 5: Images


### Adding Images


`<img> ` : To add an image into the page you need to use an <img> element. 
 It must carry the following two attributes:
 
 - `src` : This tells the browser where it can find the image file.
 - `alt` : This provides a text description of the image which describes the image if you cannot see it.
 - `title` :  Most browsers will display the content of this attribute in a tootip when the user hovers over the image.
 - `height`
 - `width`


```
<img src="images/quokka.jpg" alt="A family of
 quokka" width="600" height="450" />
 ```
 
![img](https://imgk.timesnownews.com/74666103_2454188944828540_4366738148824794550_n_1574090431__rend_1_1.jpg?tr=w-600)
 
 
### Image placement 

1. before a paragraph
2. inside the start of a paragraph
3. in the middle of a paragraph

### More attributes:

`align` :  To indicate how the other parts of a page should flow around an image. 
It has been removed from HTML5 and new websites should use CSS to control the alignment of images.

The align attribute can take these horizontal and vertical values:
  - `left`
  - `right`
  - `top`
  - `middle`
  - `bottom`
  
![align](https://www.abrightclearweb.com/wp-content/uploads/2017/03/Two-images-left-and-right-aligned-with-text.png)


### Three Rules for Creating Images

1. Save images in the right format
2. Save images at the right size
3. Use the correct resolution


### Figure and Figure Caption

`<figure>` :  HTML5 has introduced a new <figure> element to contain images and their caption
so that the two are associated. 

`<figcaption>` : To allow web page authors to add a caption to an image.

![fig](https://i.stack.imgur.com/1gpkT.png)



## Chapter 11: Color

`color` : The color property allows you to specify the color of text inside an element.

We can specify any color in CSS in one of three ways:
1. rgb values
2. hex codes
3. color names


```
/* color name */
h1 {
  color: DarkCyan;}
/* hex code */
h2 {
  color: #ee3e80;}
/* rgb value */
p {
  color: rgb(100,100,90);}
```

`background-color` :  the background-color property sets the color of the background 

```
body {
   background-color: rgb(200,200,200);}
h1 {
   background-color: DarkCyan;}
h2 {
   background-color: #ee3e80;}
p {
   background-color: white;}
```


### Understanding Color

Every color on a computer screen is created by mixing amounts of red,
green, and blue. To find the color you want, we can use a `color picker`.


![picker](https://raw.githubusercontent.com/brianpkelley/md-color-picker/master/md-color-picker-2.png)


#### Hue, Saturation and Brightness


![hue](https://3.bp.blogspot.com/-9vvvg45dX-Y/UjCNW96hbTI/AAAAAAAAAO8/jPUpBJ4fZsM/s1600/hsl-color-model.png)


### Opacity

`opacity` 
`rgba`

![op](https://lh3.googleusercontent.com/proxy/meGiUTKciH0EVXnMABdLMl9U9hrRwLO_bUKDXFoxbpnjR4cmy_gqs2cdilkrp6BUSf7oRHY7iLHGwlCusjndoGmkv4Ci_wrT0JsbaA)


## Chapter 12: Text


### Typeface Terminology


`Serif `
`Sans-Serif`
`Monospace`


![txt](https://s2.ax1x.com/2020/01/15/lXHifs.png)


`Weight` : Light Medium Bold Black
`Style` : Normal Italic Oblique
`Stretch` : Condensed Regular Extended

### Units of Type Size

`pixels: px` 
`percentage: %`
`ems: em`


![size](https://user.oc-static.com/upload/2018/04/30/15251064835155_fontsizes.png)


`@font-face` allows to use a font, even if it is not installed on the computer of the person browsing, by allowing you to specify a path to a copy of the font.

```
@font-face {
   font-family: 'ChunkFiveRegular';
   src: url('fonts/chunkfive.eot');}
h1, h2 {
   font-family: ChunkFiveRegular, Georgia, serif;}
```

### Underline & Strike

`text-decoration` :
  - `none`
  - `underline`
  - `overline`
  - `line-through`
  - `blink`
  
  
### Keywords
  
`line-height`
`letter-spacing`
`word-spacing`
`text-align`
`vertical-align`
`text-indent`
`text-shadow`
`:first-letter` 
`:first-line`
`:link` 
`:visited`
`:hover` 
`:active` 
`:focus`


### Attribute Selectors


1. Existence : `[]` Matches a specific attribute

2. Equality : `[=]` Matches a specific attribute with a specific value

3. Space : `[~=]` Matches a specific attribute whose value appears in a spaceseparated list of words

4. Prefix : `[^=]` Matches a specific attribute whose value begins with a
specific string

5. SubString : `[*=]` Matches a specific attribute whose value contains a specific
substring

6. Suffix : `[$=]` Matches a specific attribute whose value ends with a specific
string
  
  






