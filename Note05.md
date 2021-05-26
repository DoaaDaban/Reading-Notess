

#From the Duckett HTML book:

## Chapter 5: “Images” (pp.94-125)

<hr></hr>

### Adding Images:
<img> images.html HTML To add an image into the page you need to use an <img> element. This is an empty element (which means there is no closing tag). It must carry the
following two attributes:
src
This tells the browser where
it can find the image file. This
will usually be a relative URL
pointing to an image on your
own site. (Here you can see that
the images are in a child folder
called images — relative URLs
were covered on pages 83-84).
alt
This provides a text description
of the image which describes the
image if you cannot see it.
title
You can also use the title
attribute with the <img> element
to provide additional information
about the image. Most browsers
will display the content of this
attribute in a tootip when the
user hovers over the image.
Adding Images
The text used in the alt attribute
is often referred to as alt text.
It should give an accurate
description of the image content
so it can be understood by
screen reader software (used by
people with visual impairments)
and search engines.
If the image is just to make a
page look more attractive (and
it has no meaning, such as a
graphic dividing line), then the
alt attribute should still be used
but the quotes should be left
empty


### Height & Width of Images

You will also often see an <img>
element use two other attributes
that specify its size:
height
This specifies the height of the
image in pixels.
width
This specifies the width of the
image in pixels.
Images often take longer to
load than the HTML code that
makes up the rest of the page.
It is, therefore, a good idea to
specify the size of the image
so that the browser can render
the rest of the text on the page
while leaving the right amount of
space for the image that is still
loading.
The size of images is increasingly
being specified using CSS rather
than HTML — see pages 409-
410 for more information about
this.

### Where to Place Images in Your Code

Where an image is placed
in the code will affect how it
is displayed. Here are three
examples of image placement
that produce different results:
1: before a paragraph
The paragraph starts on a new
line after the image.
2: inside the start of a
paragraph
The first row of text aligns with
the bottom of the image.
3: in the middle of a
paragraph
The image is placed between the
words of the paragraph that it
appears in.


### Old Code: Aligning Images Horizontally

align horizontally.html HTML
The align attribute was
commonly used to indicate how
the other parts of a page should
flow around an image. It has
been removed from HTML5
and new websites should use
CSS to control the alignment of
images (as you will see on pages
411-412).
I have discussed it here because
you are likely to come across
it if you look at older code, and
because some visual editors still
insert this attribute when you
indicate how an image should be
aligned.
The align attribute can take
these horizontal values:
left
This aligns the image to the left
(allowing text to flow around its
right-hand side).
right
This aligns the image to the right
(allowing text to flow around its
left-hand side).

### Old Code: Aligning Images Vertically

As you saw on the last page, the
align attribute is no longer used
in HTML5, but it is covered here
because you may see it used in
older websites and it is still used
in the code created by some
visual editors.
You can see how to use CSS
to achieve the same effects on
pages 285-286.
There are three values that the
align attribute can take that
control how the image should
align vertically with the text that
surrounds it:
top
This aligns the first line of the
surrounding text with the top of
the image.
middle
This aligns the first line of the
surrounding text with the middle
of the image.
bottom
This aligns the first line of the
surrounding text with the bottom
of the image.



## Three Rules for creating Images

1- 
Save images in
the right format
Websites mainly use images in
jpeg, gif, or png format. If you
choose the wrong image
format then your image might
not look as sharp as it should
and can make the web page
slower to load.


2-
Save images at
the right size
You should save the image at
the same width and height it will
appear on the website. If
the image is smaller than the
width or height that you have
specified, the image can be
distorted and stretched. If the
image is larger than the width
and height if you have specified,
the image will take longer to
display on the page.

3-
Use the correct
resolution
Computer screens are made up
of dots known as pixels. Images
used on the web are also made
up of tiny dots. Resolution refers
to the number of dots per inch,
and most computer screens only
show web pages at 72 pixels
per inch. So saving images at
a higher resolution results in
images that are larger than
necessary and take longer to
download.


## Tools to Edit & Save Images:

1- Other Software:

* Adobe Fireworks
* Pixelmator
* PaintShop Pro
* Paint.net

2- Online Editors: 

* www.photoshop.com
* www.pixlr.com
* www.splashup.com
* www.ipiccy.com

3- Online extra

Watch videos that demonstrate
how to resize images and save
them in the correct format using
both of these applications.


## Chapter 11: “Color” (pp.246-263)

<hr></hr>

## Color
The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:

1- rgb values
These express colors in terms
of how much red, green and
blue are used to make it up. For
example: rgb(100,100,90)

2- hex codes
These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash #
sign. For example: #ee3e80

3- color names
There are 147 predefined color
names that are recognized
by browsers. For example:
DarkCyan

<hr></hr>



## Chapter 12: “Text” (pp.264-299)

Typeface Terminology:

1- Serif
Serif fonts have extra details on
the ends of the main strokes of
the letters. These details are
known as serifs.
In print, serif fonts were
traditionally used for long
passages of text because they
were considered easier to read.

2- Sans-Serif
Sans-serif fonts have straight
ends to letters, and therefore
have a much cleaner design.
Screens have a lower resolution
than print. So, if the text is small,
sans-serif fonts can be clearer
to read.

3- Monospace
Every letter in a monospace (or
fixed-width) font is the same
width. (Non-monospace fonts
have different widths.)
Monospace fonts are commonly
used for code because they align
nicely, making the text easier to
follow.

<hr></hr>

# From plog post
[JPEG vs PNG vs GIF](https://blog.imagekit.io/jpeg-vs-png-vs-gif-which-image-format-to-use-and-when-c8913ae3e01d)

## The most three commonly used image formats in websites and mobile applications is :

1- JPEG : Use JPEG format for all images that contain a natural scene or photograph where variation in colour and      i   intensity is smooth.

2- PNG : Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. 

3- GIF : Use GIF format for images that contain animations.


## Compression : can be of two types : lossless and lossy

Almost all forms of data that we see on the internet — text, image, video etc. — are compressed to reduce the size of data and ensure faster transmission. Choosing the correct format and compression is a major factor that determines image size.


## Transparency

In a simple form, transparency indicates something that is completely invisible. Logos and icons often need to be placed on backgrounds with variable colours. Hence it is desirable, that the background of these logos and icons is made transparent so that a single image can be used over multiple background variations.

* JPEG images don’t support transparency and are hence not usable for such cases.
* PNG images support transparency in two ways — inserting an alpha
* GIF images support transparency by declaring a single colour in the colour palette as transparent [index transparency](http://www.idux.com/2011/02/27/what-are-index-and-alpha-transparency/)


## Colours

Three formats:

* JPEG images can support around 16 million colours. This is what makes them suitable for storing images of natural scenes.
* PNG images mainly have two modes — PNG8 and PNG24. PNG8 can support upto 256 colours whereas PNG24 can handle upto 16 million colours like a JPEG image. Use PNG8 for simple shapes with fewer colours and PNG24 for high quality, complex logos and shapes with rounded corners on a transparent background.
* GIF images are limited to 256 colours. If index transparency is used, then one of these 256 colours is assigned as transparent and the remaining 255 are used for other colours.


## Animation

Animation, in this case, refers to any change or movement in the image. It doesn’t necessarily have to have frame rates like an animated video, but essentially a part or the entire image changes with time. 

Only GIF supports animation, This capability makes GIF format suitable for delivering engaging ads and banners. Of late, with the advent of companies Tumblr, 9Gag, Giphy etc. the use of GIF format for memes has picked up.