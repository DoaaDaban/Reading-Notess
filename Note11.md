# Readings : Audio, Video, Images

Reading

From the Duckett HTML book:

## Chapter 16: “Images” (pp.406-427)

<hr>

* Controlling size of images in CSS

HTML

```html
<img src="images/magnolia-large.jpg"
class="large" alt="Magnolia" />
<img src="images/magnolia-medium.jpg"
class="medium" alt="Magnolia" />
<img src="images/magnolia-small.jpg"
class="small" alt="Magnolia" />

```

CSS

```CSS

img.large {
width: 500px;
height: 500px;}
img.medium {
width: 250px;
height: 250px;}
img.small {
width: 100px;
height: 100px;}
```

* Aligning images in CSS

HTML

```html

<p><img src="images/magnolia-medium.jpg"
alt="Magnolia" class="align-left medium" />
<b><i>Magnolia</i></b> is a large genus that
contains over 200 flowering plant species...</p>
<p><img src="images/magnolia-medium.jpg"
alt="Magnolia" class="align-right medium" />
Some magnolias, such as <i>Magnolia stellata</i>
and <i>Magnolia soulangeana</i>, flower quite
early in the spring before the leaves open...</p>
```

CSS

```css

img.align-left {
float: left;
margin-right: 10px;}
img.align-right {
float: right;
margin-left: 10px;}
img.medium {
width: 250px;
height: 250px;}

```

* Centering images
Using css

HTML
```html
<p><img src="images/magnolia-medium.jpg"
alt="Magnolia" class="align-center medium" />
<b><i>Magnolia</i></b> is a large genus that
contains over 200 flowering plant species. It
is named after French botanist Pierre Magnol and,
having evolved before bees appeared, the
flowers were developed to encourage pollination
by beetle.</p>
```

CSS
```CSS
img.align-center {
display: block;
margin: 0px auto;}
img.medium {
width: 250px;
height: 250px;}
```

* Background Images
background-image

CSS
```CSS
body {
background-image: url("images/pattern.gif");}
```

### Repeating Images
background-repeat

* repeat : horizantally and vertically
* repeat-x : horizantally
* repeat-y : vertically 
* no-repeat: once


### The background-attachment
property specifies whether a
background image should stay in
one position or move as the user
scrolls up and down the page. It
can have one of two values:

1- fixed : The background image stays in
the same position on the page.

2- scroll : The background image moves
up and down as the user scrolls
up and down the page.


```css
body {
background-image: url("images/header.gif");
background-repeat: repeat-x;}
```
```css
body {
background-image: url("images/tulip.gif");
background-repeat: no-repeat;
background-attachment: fixed;}
```

* Background Position
background-position

```css
body {
background-image: url("images/tulip.gif");
background-repeat: no-repeat;
background-position: center top;}
```

```css
body {
background-image: url("images/tulip.gif");
background-repeat: no-repeat;
background-position: 50% 50%;}
```

* When an image is not being
repeated, you can use the
background-position
property to specify where in the
browser window the background
image should be placed.
This property usually has a pair
of values. The first represents
the horizontal position and the
second represents the vertical.

+ left top
+ left center
+ left bottom
+ center top
+ center center
+ center bottom
+ right top
+ right center
+ right bottom

### summary

* You can specify the dimensions of images using CSS.
* This is very helpful when you use the same sized
images on several pages of your site.
* Images can be aligned both horizontally and vertically
using CSS.
* You can use a background image behind the box
created by any element on a page.
* Background images can appear just once or be
repeated across the background of the box.
* You can create image rollover effects by moving the
background position of an image.
* To reduce the number of images your browser has to
load, you can create image sprites.

<hr>


## Chapter 19: “Practical Information” (476-492)

<hr>

* Search engine optimization

SEO is a huge topic and several books have been written on the subject.
The following pages will help you understand the key concepts so you can
improve your website's visibility on search engines.

- The Basics
- On-Page Techniques : In every page of your website there are seven key places where keywords
(the words people might search on to find your site) can appear in order
to improve its findability
- Off-Page Techniques


* Using analytics to understand visitors


* Putting your site on the web


### summary

* Search engine optimization helps visitors find your
sites when using search engines.
* Analytics tools such as Google Analytics allow you to
see how many people visit your site, how they find it,
and what they do when they get there.
* To put your site on the web, you will need to obtain a
domain name and web hosting.
* FTP programs allow you to transfer files from your
local computer to your web server.
* Many companies provide platforms for blogging, email
newsletters, e-commerce and other popular website
tools (to save you writing them from scratch