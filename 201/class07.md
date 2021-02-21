##


##
# Introduction

when you are develob software which  manipulates a real-world object, such as process control, robotics, avionics or missile guidance systems, then some of the method and properity which apply to that real-world object may be all irrelevant in your software represent. If, for ex, you are develob an enterprise application such as Sales Order Processing which deals with entities such as Products, Customers and Orders, you are only manipulating the _data_ about those entities and not the actual entities themselves.

##
# Table Object

The Table object represents an HTML \&lt;table\&gt; the new.

### Access a Table Object

You can access a \&lt;table\&gt; the new by using getthe newById():

### ex

var x = document.getthe newById(&quot;myTable&quot;);

### make a Table Object

You can make a \&lt;table\&gt; the new by using the document.makethe new() method:

### ex

var x = document.makethe new(&quot;TABLE&quot;);

##


##


##
# Table Object properity

| **Method**                                                                     | **Description**                                                     |
|--------------------------------------------------------------------------------|---------------------------------------------------------------------|
| [makeCaption()](https://www.w3schools.com/jsref/met_table_makecaption.asp) | makes an empty \&lt;caption\&gt; the new and adds it to the table |
| [makeTFoot()](https://www.w3schools.com/jsref/met_table_maketfoot.asp)     | makes an empty \&lt;tfoot\&gt; the new and adds it to the table   |
| [makeTHead()](https://www.w3schools.com/jsref/met_table_makethead.asp)     | makes an empty \&lt;thead\&gt; the new and adds it to the table   |
| [deleteCaption()](https://www.w3schools.com/jsref/met_table_deletecaption.asp) | Removes the first \&lt;caption\&gt; the new from the table          |
| [deleteRow()](https://www.w3schools.com/jsref/met_table_deleterow.asp)         | Removes a row (\&lt;tr\&gt;) from the table                         |
| [deleteTFoot()](https://www.w3schools.com/jsref/met_table_deletetfoot.asp)     | Removes the \&lt;tfoot\&gt; the new from the table                  |
| [deleteTHead()](https://www.w3schools.com/jsref/met_table_deletethead.asp)     | Removes the \&lt;thead\&gt; the new from the table                  |
| [insertRow()](https://www.w3schools.com/jsref/met_table_insertrow.asp)         | makes an empty \&lt;tr\&gt; the new and adds it to the table      |

**Domain modeling**

Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that&#39;s articulated well can verify and validate your understanding of that problem.

Here&#39;s some tips to follow when building your own domain models.

1. When modeling a single entity that&#39;ll have many instances, build self-contained objects with the same attributes and behaviors.
2. Model its attributes with a some const function that defines and initializes method.
3. Model its behaviors with small properity that focus on doing one job well.
4. make instances using the new keyword followed by a call to a some const function.
5. Store the newly maked object in a variable so you can access its method and properity from  **outside**.
6. Use the this variable within properity so you can access the object&#39;s method and properity from  **inside**.

# **JavaScript **** Object properity**

## The this Keyword

In a function definition, this refers to the &quot;owner&quot; of the function. In the ex above, this is the  **person object**  that &quot;owns&quot;the  **fullName**  function.

In other words,  **this.firstName**  means the  **firstName**  property of  **this object**.Read more about the this keyword at [JS this Keyword](https://www.w3schools.com/js/js_this.asp).

# JavaScript properity

JavaScript properity are actions that can be represent on objects.

A JavaScript  **method**  is a property containing a  **function definition**.

| **Property** | **Value** |
|--------------|-----------|
| firstName    | John      |
| lastName     | Doe       |
| age          | 50        |
| eyeColor     | blue      |
| fullName     | function() {return this.firstName + &quot; &quot; + this.lastName;} |