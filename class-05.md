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

![fig](https://freefrontend.com/assets/img/html-figure-and-figcapture-with-css/Picture-Cards-Figure-Figcaption.jpg)



