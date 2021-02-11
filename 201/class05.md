# Definition and Usage

The \&lt;img\&gt; tag is used to embed an image in an HTML page.

Images are not technically inserted into a web page; images are linked to web pages. The \&lt;img\&gt; tag creates a holding space for the referenced image.

The \&lt;img\&gt; tag has two required attributes:

- src - Specifies the path to the image
- alt - Specifies an alternate text for the image, if the image for some reason cannot be displayed

# HTML \&lt;img\&gt; Tag

\&lt;img src=&quot;img.jpg&quot; alt=&quot;&quot; width=&quot;&quot; height=&quot;&quot;\&gt;

Align image (with CSS):

\&lt;img src=&quot;smiley.gif&quot; alt=&quot;Smiley face&quot; width=&quot;42&quot; height=&quot;42&quot; style=&quot;vertical-align:bottom&quot;\&gt;

Add image border (with CSS):

\&lt;img src=&quot;smiley.gif&quot; alt=&quot;Smiley face&quot; width=&quot;42&quot; height=&quot;42&quot; style=&quot;border:5px solid black&quot;\&gt;

Add left and right margins to image (with CSS):

\&lt;img src=&quot;smiley.gif&quot; alt=&quot;Smiley face&quot; width=&quot;42&quot; height=&quot;42&quot; style=&quot;vertical-align:middle;margin:0px 50px&quot;\&gt;

How to insert images from another folder or from another web site:

\&lt;img src=&quot;/images/stickman.gif&quot; alt=&quot;Stickman&quot; width=&quot;24&quot; height=&quot;39&quot;\&gt;

How to add a hyperlink to an image:

\&lt;a href=&quot;https://www.w3schools.com&quot;\&gt;
\&lt;img src=&quot;w3html.gif&quot; alt=&quot;W3Schools.com&quot; width=&quot;100&quot; height=&quot;132&quot;\&gt;
\&lt;/a\&gt;

## img {
  display: inline-block;
}

## Text Color

The color property is used to set the color of the text. The color is specified by:

- a color name - like &quot;red&quot;
- a HEX value - like &quot;#ff0000&quot;
- an RGB value - like &quot;rgb(255,0,0)&quot;

Most browsers will display the \&lt;img\&gt; element with the following default values:

### Example

body {
  color: blue;
}

h1 {
  color: green;
}

## Text Color and Background Color

### Example

### body {
  background-color: lightgrey;
  color: blue;
}

h1 {
  background-color: black;
  color: white;
}