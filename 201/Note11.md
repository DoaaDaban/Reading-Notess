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

<hr>

from [This MDN article on audio and video elements](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs)


## Video and Audio APIs
HTML5 comes with elements for embedding rich media in documents —``` <video> ```and ``` <audio>``` — which in turn come with their own APIs for controlling playback, seeking, etc. This article shows you how to do common tasks such as creating custom playback controls.

Prerequisites:	JavaScript basics (see first steps, building blocks, JavaScript objects), the basics of Client-side APIs

Objective:	To learn how to use browser APIs to control video and audio playback.

HTML5 video and audio

The ```<video>``` and ```<audio>``` elements allow us to embed video and audio into web pages. As we showed in Video and audio content, a typical implementation looks like this:

```HTML
<video controls>
  <source src="rabbit320.mp4" type="video/mp4">
  <source src="rabbit320.webm" type="video/webm">
  <p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
</video>
```
This creates a video player inside the browser.

### The HTMLMediaElement API

Part of the HTML5 spec, the [HTMLMediaElement](https://developer.mozilla.org/en-US/docs/Web/API/HTMLMediaElement) API provides features to allow you to control video and audio players programmatically — for example [HTMLMediaElement.play()](https://developer.mozilla.org/en-US/docs/Web/API/HTMLMediaElement/play), [HTMLMediaElement.pause()](https://developer.mozilla.org/en-US/docs/Web/API/HTMLMediaElement/pause), etc. This interface is available to both ``` <audio>``` and ``` <video>``` elements, as the features you'll want to implement are nearly identical. Let's go through an example, adding features as we go.


<hr>

## Chapter 9: pages 201-206 only. Flash is no longer supported by many browsers but is an important part of history.

* How to add Flash movies into your site
* How to add video and audio to your site
* HTML5 ```<video>``` and ```<audio>``` elements

Flash is a very popular technology used
to add animations, video, and audio to
websites. This chapter begins by looking
at how to use it in your web pages.
We then focus on how to add video and audio to your site,
using either the new HTML5 ```<video>``` and ```<audio>``` elements
or a hosted service (such as YouTube or SoundCloud). In this
chapter you will learn:

●● How to use Flash in your web pages

●● How to use HTML5 ``` <video>``` and ```<audio>``` elements

●● When to host your own video and audio and when to use a
service such as YouTube

![Timeline:
Flash, VidEo & Audio](https://aleen42.gitbooks.io/wiki/content/Programming/HTML/flash_video_audio/timeline.png)

### Adding a Flash Movie to Your Web Page

```html
<!DOCTYPE html>
<html>
<head>
<title>Adding a Flash Movie</title>
<script type="text/javascript"
src="http://ajax.googleapis.com/ajax/libs/
swfobject/2.2/swfobject.js"></script>
<script type="text/javascript">
swfobject.embedSWF("flash/bird.swf",
"bird", "400", "300", "8.0.0");</script>
</head>
<body>
<div id="bird"><p>An animation of a bird taking
a shower</p></div>
</body>
</html>

```



### Example flash & AUdio & video 

```html
<!DOCTYPE html>
<html>
<head>
<title>Flash, Video and Audio</title>
<script type="text/javascript"
src="http://ajax.googleapis.com/ajax/libs/
swfobject/2.2/swfobject.js"></script>
<script type="text/javascript">
var flashvars = {};
var params = {movie: "../video/puppy.flv"};
swfobject.embedSWF("flash/osplayer.swf", "snow",
"400", "320", "8.0.0", flashvars, params);</script>
</head>
<body>
<video poster="images/puppy.jpg" width="400"
height="320" controls="controls">
<source src="video/puppy.mp4" type='video/mp4;
codecs="avc1.42E01E, mp4a.40.2"' />
<source src="video/puppy.webm" type='video/webm;
codecs="vp8, vorbis"' />
<div id="snow">
<p>You cannot see this video of a puppy playing
in the snow because this browser does not
support our video formats.</p>
</div>
</video>
</body>
</html>
```

### summary
* Flash allows you to add animations, video and audio to
the web.
* Flash is not supported on iPhone or iPad.
* HTML5 introduces new ```<video>``` and ```<audio>```
elements for adding video and audio to web pages, but
these are only supported in the latest browsers.
* Browsers that support the HTML5 elements do not
all support the same video and audio formats, so you
need to supply your files in different formats to ensure
that everyone can see/hear them