##
# HTML Links - Syntax

The HTML \&lt;a\&gt; tag defines a hyperlink. It has the following syntax:

\&lt;a href=&quot;_url_&quot;\&gt;_link text_\&lt;/a\&gt;

The most important attribute of the \&lt;a\&gt; element is the href attribute, which indicates the link&#39;s destination.

The _link text_ is the part that will be visible to the reader.

Clicking on the link text, will send the reader to the specified URL address.

HTML Links - The target Attribute

By default, the linked page will be displayed in the current browser window. To change this, you must specify another target for the link.

The target attribute specifies where to open the linked document.

The target attribute can have one of the following values:

- \_self - Default. Opens the document in the same window/tab as it was clicked
- \_blank - Opens the document in a new window or tab
- \_parent - Opens the document in the parent frame
- \_top - Opens the document in the full body of the window

Example

Use target=&quot;\_blank&quot; to open the linked document in a new browser window or tab:

## HTML Links - Use an Image as a Link

To use an image as a link, just put the \&lt;img\&gt; tag inside the \&lt;a\&gt; tag:

# Links used to activate JavaScript functions

## Which &quot;href&quot; value should I use for JavaScript links, &quot;#&quot; or &quot;javascript:void(0)&quot;?

**Published Sep 21, 2019**

When you are creating an app using plain JavaScript, sometimes you&#39;ll have the necessity of triggering a function when the user clicks a link.

You can commonly do this in 2 ways.

Suppose the function you want to execute is called handleClick():

functionhandleClick(){

alert(&#39;clicked&#39;)

}

The first way is to use a link like this:

\&lt;a href=&quot;#&quot; onclick=&quot;handleClick()&quot;\&gt;Click here\&lt;/a\&gt;

The second way is to use

\&lt;a href=&quot;javascript:void(0)&quot; onclick=&quot;handleClick()&quot;\&gt;Click here\&lt;/a\&gt;

They are both very similar syntaxes, the only difference is the href attribute value.

The first is href=&quot;#&quot;, the second is href=&quot;javascript:void(0)&quot;. You might also see this syntax href=&quot;javascript:;&quot;, which is equivalent to the second.

Now, what is the difference in the behavior of those 2 methods?

When the user clicks the href=&quot;#&quot; link, you _must_ make sure that you return false from the event handler, the otherwise the browser scrolls back to the top of the page:

functionhandleClick(){

alert(&#39;clicked&#39;)

returnfalse

}

Also, even if you add this but JavaScript is disabled or does not execute for some reason, the browser scrolls back to the top of the page. This is almost always a thing to avoid, so I would personally use the second form, href=&quot;javascript:void(0)&quot;.

In both ways the handleClick() function would not be called if JavaScript is disabled, or there is an error in the JavaScript and so JavaScript execution is halted.

To prevent this, you can use a real URL in the href as a fallback, so browsers will move the user to a specific page, using the GET HTTP method, although this is not always possible or convenient.

# Summary

- Use the \&lt;a\&gt; element to define a link
- Use the href attribute to define the link address
- Use the target attribute to define where to open the linked document
- Use the \&lt;img\&gt; element (inside \&lt;a\&gt;) to use an image as a link
- Use the mailto: scheme inside the href attribute to create a link that opens the user&#39;s email program

CSS layout

This article will recap some of the CSS layout features we&#39;ve already touched upon in previous modules — such as different [display](https://developer.mozilla.org/en-US/docs/Web/CSS/display) values — and introduce some of the concepts we&#39;ll be covering throughout this module.

| **Prerequisites:** | The basics of HTML (study [Introduction to HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML)), and an idea of How CSS works (study [Introduction to CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps).) |
| --- | --- |
| **Objective:** | To give you an overview of CSS page layout techniques. Each technique can be learned in greater detail in subsequent tutorials. |

CSS page layout techniques allow us to take elements contained in a web page and control where they are positioned relative to their default position in normal layout flow, the other elements around them, their parent container, or the main viewport/window.  The page layout techniques we&#39;ll be covering in more detail in this module are

- Normal flow
- The [display](https://developer.mozilla.org/en-US/docs/Web/CSS/display) property
- Flexbox
- Grid
- Floats
- Positioning
- Table layout
- Multiple-column layout

Each technique has its uses, advantages, and disadvantages, and no technique is designed to be used in isolation. By understanding what each method is designed for you will be in a good place to understand which is the best layout tool for each task

## [The display property](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Introduction#the_display_property)

The main methods of achieving page layout in CSS are all values of the display property. This property allows us to change the default way something displays. Everything in normal flow has a value of display, used as the default way that elements they are set on behave. For example, the fact that paragraphs in English display one below the other is due to the fact that they are styled with display: block. If you create a link around some text inside a paragraph, that link remains inline with the rest of the text, and doesn&#39;t break onto a new line. This is because the [\&lt;a\&gt;](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a) element is display: inline by default.

You can change this default display behavior. For example, the [\&lt;li\&gt;](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/li) element is display: block by default, meaning that list items display one below the other in our English document. If we change the display value to inline they now display next to each other, as words would do in a sentence. The fact that you can change the value of display for any element means that you can pick HTML elements for their semantic meaning, without being concerned about how they will look. The way they look is something that you can change.

In addition to being able to change the default presentation by turning an item from block to inline and vice versa, there are some bigger layout methods that start out as a value of display. However, when using these, you will generally need to invoke additional properties. The two values most important for our purposes when discussing layout are display: flex and display: grid.