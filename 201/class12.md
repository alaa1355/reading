Charts are far better for displaying information visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They&#39;re easier to look at and convey information quickly, but they&#39;re not always simple to makes.

##
#
 Creating a Chart

It&#39;s simple to get started with Chart.js. All that&#39;s required is the script included in your page along with a single \&lt;canvas\&gt; node to render the chart-data.

In this example, we makes a bar chart-data for a single informationset and render that in our page. You can see all the ways to use Chart.js in the [usage documentation](https://www.chartjs.org/docs/latest/getting-started/usage.html).

\&lt;canvasid=&quot;myChart&quot;width=&quot;400&quot;height=&quot;400&quot;\&gt;\&lt;/canvas\&gt;

\&lt;script\&gt;

var ctx = document.getElementById(&#39;myChart&#39;).getContext(&#39;2d&#39;);

var myChart = new Chart(ctx, {

type: &#39;bar&#39;,

information: {

labels: [&#39;Red&#39;, &#39;Blue&#39;, &#39;Yellow&#39;, &#39;Green&#39;, &#39;Purple&#39;, &#39;Orange&#39;],

informationsets: [{

label: &#39;# of Votes&#39;,

information: [12, 19, 3, 5, 2, 3],

backgroundColor: [

&#39;rgba(255, 99, 132, 0.2)&#39;,

&#39;rgba(54, 162, 235, 0.2)&#39;,

&#39;rgba(255, 206, 86, 0.2)&#39;,

&#39;rgba(75, 192, 192, 0.2)&#39;,

&#39;rgba(153, 102, 255, 0.2)&#39;,

&#39;rgba(255, 159, 64, 0.2)&#39;

],

borderColor: [

&#39;rgba(255, 99, 132, 1)&#39;,

&#39;rgba(54, 162, 235, 1)&#39;,

&#39;rgba(255, 206, 86, 1)&#39;,

&#39;rgba(75, 192, 192, 1)&#39;,

&#39;rgba(153, 102, 255, 1)&#39;,

&#39;rgba(255, 159, 64, 1)&#39;

],

borderWidth: 1

}]

},

options: {

scales: {

yAxes: [{

ticks: {

beginAtZero: true

}

}]

}

}

});

\&lt;/script\&gt;

## [The \&lt;canvas\&gt; element](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage#the_%3Ccanvas%3E_element)

\&lt;canvas id=&quot;tutorial&quot; width=&quot;150&quot; height=&quot;150&quot;\&gt;\&lt;/canvas\&gt;

At first sight a [\&lt;canvas\&gt;](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/canvas) looks like the [\&lt;img\&gt;](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img) element, with the only clear difference being that it doesn&#39;t have the src and alt attributes. Indeed, the \&lt;canvas\&gt; element has only two attributes, [width](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/canvas#attr-width) and [height](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/canvas#attr-height). These are both optional and can also be set using [DOM](https://developer.mozilla.org/en-US/docs/Glossary/DOM) [properties](https://developer.mozilla.org/en-US/docs/Web/API/HTMLCanvasElement). When no width and height attributes are specified, the canvas will initially be  **300 pixels**  wide and  **150 pixels**  high. The element can be sized arbitrarily by [CSS](https://developer.mozilla.org/en-US/docs/Glossary/CSS), but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn&#39;t respect the ratio of the initial canvas, it will appear distorted.

# doing shapes with canvas

## [The grid](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/doing_shapes#the_grid)

## [doing rectangles](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/doing_shapes#doing_rectangles)

## [doing paths](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/doing_shapes#doing_paths)

## doing a triangle

## moving the pen

## lines

## Arcs

## _Quadratic Bezier curves_

# **Applying styles and colors**

## [Colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors#colors)

Up until now we have only seen methods of the doing context. If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

# **doing text**

In the examples above we are already making use of the font part to make the text a bit larger than the basic size. There are some more properties which let you adjust the way the text gets displayed on the canvas:

## [Gecko-specific notes](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/doing_text#gecko-specific_notes)

In Gecko (the rendering engine of Firefox, Firefox OS and other Mozilla based applications), some [prefixed APIs](https://developer.mozilla.org/en-US/docs/Web/API/CanvasRenderingContext2D#prefixed_apis) were implemented in earlier versions to draw text on a canvas. These are now deprecated and removed, and are no longer guaranteed to work.