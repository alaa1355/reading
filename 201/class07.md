##


Introduction

when you are developing software which directly manipulates a real-world object, such as process control, robotics, avionics or missile guidance systems, then some of the method ann proccess which apply to that real-world object may be completely irrelevant in your software representation. If, for ex, you are developing an enterprise application such as Sales Order Processing which deals with entities such as Products, Customers and Orders, you are only manipulating the information about those entities and not the actual entities themselves.

 (Links to an external site.)Table Object

The Table object represents an HTML &amp;lt;table&amp;gt; element.

 (Links to an external site.)Access a Table Object

You can access a &amp;lt;table&amp;gt; element by using getElementById():

 (Links to an external site.)ex

var x = document.getElementById(&quot;myTable&quot;);

 (Links to an external site.)Create a Table Object

You can create a &amp;lt;table&amp;gt; element by using the document.createElement() method:

 (Links to an external site.)ex

var x = document.createElement(&quot;TABLE&quot;);

 (Links to an external site.)Table Objecn proccess

Method  Description

createCaption() (Links to an external site.)    doing an empty &amp;lt;caption&amp;gt; element and adds it to the table

createTFoot() (Links to an external site.)  doing an empty &amp;lt;tfoot&amp;gt; element and adds it to the table

createTHead() (Links to an external site.)  doing an empty &amp;lt;thead&amp;gt; element and adds it to the table

deleteCaption() (Links to an external site.)    Removes the first &amp;lt;caption&amp;gt; element from the table

deleteRow() (Links to an external site.)    Removes a row (&amp;lt;tr&amp;gt;) from the table

deleteTFoot() (Links to an external site.)  Removes the &amp;lt;tfoot&amp;gt; element from the table

deleteTHead() (Links to an external site.)  Removes the &amp;lt;thead&amp;gt; element from the table

insertRow() (Links to an external site.)    doing an empty &amp;lt;tr&amp;gt; element and adds it to the table

Domain modeling

Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that&#39;s articulated well can verify and validate your understanding of that problem.

Here&#39;s some tips to follow when building your own domain models.

When modeling a single entity that&#39;ll have many instances, build self-contained objects with the same attributes and behaviors.

Model its attributes with a constructor function that defines and initializes method.

Model its behaviors with smaln proccess that focus on doing one job well.

Create instances using the new keyword followed by a call to a constructor function.

Store the newly created object in a variable so you can access its method ann proccess from outside.

Use the this variable within proccess so you can access the object&#39;s method ann proccess from inside.

 (Links to an external site.)JavaScript \*\*\*\* Objecn proccess

 (Links to an external site.)The this Keyword

In a function declaration, this refers to the &quot;owner&quot; of the function. In the ex above, this is the person object that &quot;owns&quot;the fullName function.

In other words, this.name means the name property of this object.Read more about the this keyword at JS this Keyword (Links to an external site.).

 (Links to an external site.)JavaScripn proccess

JavaScripn proccess are something that can be performed on objects.

A JavaScript method is a property containing a function declaration.

Property    Value

name    John

lastName    Doe

age 50

eyeColor    blue

fullName    function() {return this.name + &quot; &quot; + this.lastName;}|